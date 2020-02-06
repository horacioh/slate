
# External module: "interfaces/node"

## Index

### Type aliases

* [Ancestor](_interfaces_node_.md#ancestor)
* [Descendant](_interfaces_node_.md#descendant)
* [Node](_interfaces_node_.md#node)
* [NodeEntry](_interfaces_node_.md#nodeentry)

### Object literals

* [Node](_interfaces_node_.md#const-node)

## Type aliases

###  Ancestor

Ƭ **Ancestor**: *[Editor](../interfaces/_interfaces_editor_.editor.md) | [Element](../interfaces/_interfaces_element_.element.md)*

The `Ancestor` union type represents nodes that are ancestors in the tree.
It is returned as a convenience in certain cases to narrow a value further
than the more generic `Node` union.

___

###  Descendant

Ƭ **Descendant**: *[Element](../interfaces/_interfaces_element_.element.md) | [Text](../interfaces/_interfaces_text_.text.md)*

The `Descendant` union type represents nodes that are descendants in the
tree. It is returned as a convenience in certain cases to narrow a value
further than the more generic `Node` union.

___

###  Node

Ƭ **Node**: *[Editor](../interfaces/_interfaces_editor_.editor.md) | [Element](../interfaces/_interfaces_element_.element.md) | [Text](../interfaces/_interfaces_text_.text.md)*

The `Node` union type represents all of the different types of nodes that
occur in a Slate document tree.

___

###  NodeEntry

Ƭ **NodeEntry**: *[T, [Path](_interfaces_path_.md#path)]*

`NodeEntry` objects are returned when iterating over the nodes in a Slate
document tree. They consist of the node and its `Path` relative to the root
node in the document.

## Object literals

### `Const` Node

### ▪ **Node**: *object*

###  ancestor

▸ **ancestor**(`root`: [Node](_interfaces_node_.md#node), `path`: [Path](_interfaces_path_.md#path)): *[Ancestor](_interfaces_node_.md#ancestor)*

Get the node at a specific path, asserting that it's an ancestor node.

**Parameters:**

Name | Type |
------ | ------ |
`root` | [Node](_interfaces_node_.md#node) |
`path` | [Path](_interfaces_path_.md#path) |

**Returns:** *[Ancestor](_interfaces_node_.md#ancestor)*

###  ancestors

▸ **ancestors**(`root`: [Node](_interfaces_node_.md#node), `path`: [Path](_interfaces_path_.md#path), `options`: object): *Iterable‹[NodeEntry](_interfaces_node_.md#nodeentry)‹[Ancestor](_interfaces_node_.md#ancestor)››*

Return an iterable of all the ancestor nodes above a specific path.

By default the order is bottom-up, from lowest to highest ancestor in
the tree, but you can pass the `reverse: true` option to go top-down.

**Parameters:**

▪ **root**: *[Node](_interfaces_node_.md#node)*

▪ **path**: *[Path](_interfaces_path_.md#path)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`reverse?` | boolean |

**Returns:** *Iterable‹[NodeEntry](_interfaces_node_.md#nodeentry)‹[Ancestor](_interfaces_node_.md#ancestor)››*

###  child

▸ **child**(`root`: [Node](_interfaces_node_.md#node), `index`: number): *[Descendant](_interfaces_node_.md#descendant)*

Get the child of a node at a specific index.

**Parameters:**

Name | Type |
------ | ------ |
`root` | [Node](_interfaces_node_.md#node) |
`index` | number |

**Returns:** *[Descendant](_interfaces_node_.md#descendant)*

###  children

▸ **children**(`root`: [Node](_interfaces_node_.md#node), `path`: [Path](_interfaces_path_.md#path), `options`: object): *Iterable‹[NodeEntry](_interfaces_node_.md#nodeentry)‹[Descendant](_interfaces_node_.md#descendant)››*

Iterate over the children of a node at a specific path.

**Parameters:**

▪ **root**: *[Node](_interfaces_node_.md#node)*

▪ **path**: *[Path](_interfaces_path_.md#path)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`reverse?` | boolean |

**Returns:** *Iterable‹[NodeEntry](_interfaces_node_.md#nodeentry)‹[Descendant](_interfaces_node_.md#descendant)››*

###  common

▸ **common**(`root`: [Node](_interfaces_node_.md#node), `path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *[NodeEntry](_interfaces_node_.md#nodeentry)*

Get an entry for the common ancesetor node of two paths.

**Parameters:**

Name | Type |
------ | ------ |
`root` | [Node](_interfaces_node_.md#node) |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *[NodeEntry](_interfaces_node_.md#nodeentry)*

###  descendant

▸ **descendant**(`root`: [Node](_interfaces_node_.md#node), `path`: [Path](_interfaces_path_.md#path)): *[Descendant](_interfaces_node_.md#descendant)*

Get the node at a specific path, asserting that it's a descendant node.

**Parameters:**

Name | Type |
------ | ------ |
`root` | [Node](_interfaces_node_.md#node) |
`path` | [Path](_interfaces_path_.md#path) |

**Returns:** *[Descendant](_interfaces_node_.md#descendant)*

###  descendants

▸ **descendants**(`root`: [Node](_interfaces_node_.md#node), `options`: object): *Iterable‹[NodeEntry](_interfaces_node_.md#nodeentry)‹[Descendant](_interfaces_node_.md#descendant)››*

Return an iterable of all the descendant node entries inside a root node.

**Parameters:**

▪ **root**: *[Node](_interfaces_node_.md#node)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`from?` | [Path](_interfaces_path_.md#path) |
`pass?` | function |
`reverse?` | boolean |
`to?` | [Path](_interfaces_path_.md#path) |

**Returns:** *Iterable‹[NodeEntry](_interfaces_node_.md#nodeentry)‹[Descendant](_interfaces_node_.md#descendant)››*

###  elements

▸ **elements**(`root`: [Node](_interfaces_node_.md#node), `options`: object): *Iterable‹[ElementEntry](_interfaces_element_.md#elemententry)›*

Return an iterable of all the element nodes inside a root node. Each iteration
will return an `ElementEntry` tuple consisting of `[Element, Path]`. If the
root node is an element it will be included in the iteration as well.

**Parameters:**

▪ **root**: *[Node](_interfaces_node_.md#node)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`from?` | [Path](_interfaces_path_.md#path) |
`pass?` | function |
`reverse?` | boolean |
`to?` | [Path](_interfaces_path_.md#path) |

**Returns:** *Iterable‹[ElementEntry](_interfaces_element_.md#elemententry)›*

###  first

▸ **first**(`root`: [Node](_interfaces_node_.md#node), `path`: [Path](_interfaces_path_.md#path)): *[NodeEntry](_interfaces_node_.md#nodeentry)*

Get the first node entry in a root node from a path.

**Parameters:**

Name | Type |
------ | ------ |
`root` | [Node](_interfaces_node_.md#node) |
`path` | [Path](_interfaces_path_.md#path) |

**Returns:** *[NodeEntry](_interfaces_node_.md#nodeentry)*

###  fragment

▸ **fragment**(`root`: [Node](_interfaces_node_.md#node), `range`: [Range](../interfaces/_interfaces_range_.range.md)): *[Descendant](_interfaces_node_.md#descendant)[]*

Get the sliced fragment represented by a range inside a root node.

**Parameters:**

Name | Type |
------ | ------ |
`root` | [Node](_interfaces_node_.md#node) |
`range` | [Range](../interfaces/_interfaces_range_.range.md) |

**Returns:** *[Descendant](_interfaces_node_.md#descendant)[]*

###  get

▸ **get**(`root`: [Node](_interfaces_node_.md#node), `path`: [Path](_interfaces_path_.md#path)): *[Node](_interfaces_node_.md#node)*

Get the descendant node referred to by a specific path. If the path is an
empty array, it refers to the root node itself.

**Parameters:**

Name | Type |
------ | ------ |
`root` | [Node](_interfaces_node_.md#node) |
`path` | [Path](_interfaces_path_.md#path) |

**Returns:** *[Node](_interfaces_node_.md#node)*

###  has

▸ **has**(`root`: [Node](_interfaces_node_.md#node), `path`: [Path](_interfaces_path_.md#path)): *boolean*

Check if a descendant node exists at a specific path.

**Parameters:**

Name | Type |
------ | ------ |
`root` | [Node](_interfaces_node_.md#node) |
`path` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  isNode

▸ **isNode**(`value`: any): *value is Node*

Check if a value implements the `Node` interface.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is Node*

###  isNodeList

▸ **isNodeList**(`value`: any): *value is Node[]*

Check if a value is a list of `Node` objects.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is Node[]*

###  last

▸ **last**(`root`: [Node](_interfaces_node_.md#node), `path`: [Path](_interfaces_path_.md#path)): *[NodeEntry](_interfaces_node_.md#nodeentry)*

Get the lash node entry in a root node from a path.

**Parameters:**

Name | Type |
------ | ------ |
`root` | [Node](_interfaces_node_.md#node) |
`path` | [Path](_interfaces_path_.md#path) |

**Returns:** *[NodeEntry](_interfaces_node_.md#nodeentry)*

###  leaf

▸ **leaf**(`root`: [Node](_interfaces_node_.md#node), `path`: [Path](_interfaces_path_.md#path)): *[Text](../interfaces/_interfaces_text_.text.md)*

Get the node at a specific path, ensuring it's a leaf text node.

**Parameters:**

Name | Type |
------ | ------ |
`root` | [Node](_interfaces_node_.md#node) |
`path` | [Path](_interfaces_path_.md#path) |

**Returns:** *[Text](../interfaces/_interfaces_text_.text.md)*

###  levels

▸ **levels**(`root`: [Node](_interfaces_node_.md#node), `path`: [Path](_interfaces_path_.md#path), `options`: object): *Iterable‹[NodeEntry](_interfaces_node_.md#nodeentry)›*

Return an iterable of the in a branch of the tree, from a specific path.

By default the order is top-down, from lowest to highest node in the tree,
but you can pass the `reverse: true` option to go bottom-up.

**Parameters:**

▪ **root**: *[Node](_interfaces_node_.md#node)*

▪ **path**: *[Path](_interfaces_path_.md#path)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`reverse?` | boolean |

**Returns:** *Iterable‹[NodeEntry](_interfaces_node_.md#nodeentry)›*

###  matches

▸ **matches**(`node`: [Node](_interfaces_node_.md#node), `props`: Partial‹[Node](_interfaces_node_.md#node)›): *boolean*

Check if a node matches a set of props.

**Parameters:**

Name | Type |
------ | ------ |
`node` | [Node](_interfaces_node_.md#node) |
`props` | Partial‹[Node](_interfaces_node_.md#node)› |

**Returns:** *boolean*

###  nodes

▸ **nodes**(`root`: [Node](_interfaces_node_.md#node), `options`: object): *Iterable‹[NodeEntry](_interfaces_node_.md#nodeentry)›*

Return an iterable of all the node entries of a root node. Each entry is
returned as a `[Node, Path]` tuple, with the path referring to the node's
position inside the root node.

**Parameters:**

▪ **root**: *[Node](_interfaces_node_.md#node)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`from?` | [Path](_interfaces_path_.md#path) |
`pass?` | function |
`reverse?` | boolean |
`to?` | [Path](_interfaces_path_.md#path) |

**Returns:** *Iterable‹[NodeEntry](_interfaces_node_.md#nodeentry)›*

###  parent

▸ **parent**(`root`: [Node](_interfaces_node_.md#node), `path`: [Path](_interfaces_path_.md#path)): *[Ancestor](_interfaces_node_.md#ancestor)*

Get the parent of a node at a specific path.

**Parameters:**

Name | Type |
------ | ------ |
`root` | [Node](_interfaces_node_.md#node) |
`path` | [Path](_interfaces_path_.md#path) |

**Returns:** *[Ancestor](_interfaces_node_.md#ancestor)*

###  string

▸ **string**(`node`: [Node](_interfaces_node_.md#node)): *string*

Get the concatenated text string of a node's content.

Note that this will not include spaces or line breaks between block nodes.
It is not a user-facing string, but a string for performing offset-related
computations for a node.

**Parameters:**

Name | Type |
------ | ------ |
`node` | [Node](_interfaces_node_.md#node) |

**Returns:** *string*

###  texts

▸ **texts**(`root`: [Node](_interfaces_node_.md#node), `options`: object): *Iterable‹[NodeEntry](_interfaces_node_.md#nodeentry)‹[Text](../interfaces/_interfaces_text_.text.md)››*

Return an iterable of all leaf text nodes in a root node.

**Parameters:**

▪ **root**: *[Node](_interfaces_node_.md#node)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`from?` | [Path](_interfaces_path_.md#path) |
`pass?` | function |
`reverse?` | boolean |
`to?` | [Path](_interfaces_path_.md#path) |

**Returns:** *Iterable‹[NodeEntry](_interfaces_node_.md#nodeentry)‹[Text](../interfaces/_interfaces_text_.text.md)››*
