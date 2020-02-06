
# External module: "interfaces/operation"

## Index

### Type aliases

* [InsertNodeOperation](_interfaces_operation_.md#insertnodeoperation)
* [InsertTextOperation](_interfaces_operation_.md#inserttextoperation)
* [MergeNodeOperation](_interfaces_operation_.md#mergenodeoperation)
* [MoveNodeOperation](_interfaces_operation_.md#movenodeoperation)
* [NodeOperation](_interfaces_operation_.md#nodeoperation)
* [Operation](_interfaces_operation_.md#operation)
* [RemoveNodeOperation](_interfaces_operation_.md#removenodeoperation)
* [RemoveTextOperation](_interfaces_operation_.md#removetextoperation)
* [SelectionOperation](_interfaces_operation_.md#selectionoperation)
* [SetNodeOperation](_interfaces_operation_.md#setnodeoperation)
* [SetSelectionOperation](_interfaces_operation_.md#setselectionoperation)
* [SplitNodeOperation](_interfaces_operation_.md#splitnodeoperation)
* [TextOperation](_interfaces_operation_.md#textoperation)

### Object literals

* [Operation](_interfaces_operation_.md#const-operation)

## Type aliases

###  InsertNodeOperation

Ƭ **InsertNodeOperation**: *object*

#### Type declaration:

* \[ **key**: *string*\]: any

* **node**: *[Node](_interfaces_node_.md#node)*

* **path**: *[Path](_interfaces_path_.md#path)*

* **type**: *"insert_node"*

___

###  InsertTextOperation

Ƭ **InsertTextOperation**: *object*

#### Type declaration:

* \[ **key**: *string*\]: any

* **offset**: *number*

* **path**: *[Path](_interfaces_path_.md#path)*

* **text**: *string*

* **type**: *"insert_text"*

___

###  MergeNodeOperation

Ƭ **MergeNodeOperation**: *object*

#### Type declaration:

* \[ **key**: *string*\]: any

* **path**: *[Path](_interfaces_path_.md#path)*

* **position**: *number*

* **properties**: *Partial‹[Node](_interfaces_node_.md#node)›*

* **target**: *number | null*

* **type**: *"merge_node"*

___

###  MoveNodeOperation

Ƭ **MoveNodeOperation**: *object*

#### Type declaration:

* \[ **key**: *string*\]: any

* **newPath**: *[Path](_interfaces_path_.md#path)*

* **path**: *[Path](_interfaces_path_.md#path)*

* **type**: *"move_node"*

___

###  NodeOperation

Ƭ **NodeOperation**: *[InsertNodeOperation](_interfaces_operation_.md#insertnodeoperation) | [MergeNodeOperation](_interfaces_operation_.md#mergenodeoperation) | [MoveNodeOperation](_interfaces_operation_.md#movenodeoperation) | [RemoveNodeOperation](_interfaces_operation_.md#removenodeoperation) | [SetNodeOperation](_interfaces_operation_.md#setnodeoperation) | [SplitNodeOperation](_interfaces_operation_.md#splitnodeoperation)*

___

###  Operation

Ƭ **Operation**: *[NodeOperation](_interfaces_operation_.md#nodeoperation) | [SelectionOperation](_interfaces_operation_.md#selectionoperation) | [TextOperation](_interfaces_operation_.md#textoperation)*

`Operation` objects define the low-level instructions that Slate editors use
to apply changes to their internal state. Representing all changes as
operations is what allows Slate editors to easily implement history,
collaboration, and other features.

___

###  RemoveNodeOperation

Ƭ **RemoveNodeOperation**: *object*

#### Type declaration:

* \[ **key**: *string*\]: any

* **node**: *[Node](_interfaces_node_.md#node)*

* **path**: *[Path](_interfaces_path_.md#path)*

* **type**: *"remove_node"*

___

###  RemoveTextOperation

Ƭ **RemoveTextOperation**: *object*

#### Type declaration:

* \[ **key**: *string*\]: any

* **offset**: *number*

* **path**: *[Path](_interfaces_path_.md#path)*

* **text**: *string*

* **type**: *"remove_text"*

___

###  SelectionOperation

Ƭ **SelectionOperation**: *[SetSelectionOperation](_interfaces_operation_.md#setselectionoperation)*

___

###  SetNodeOperation

Ƭ **SetNodeOperation**: *object*

#### Type declaration:

* \[ **key**: *string*\]: any

* **newProperties**: *Partial‹[Node](_interfaces_node_.md#node)›*

* **path**: *[Path](_interfaces_path_.md#path)*

* **properties**: *Partial‹[Node](_interfaces_node_.md#node)›*

* **type**: *"set_node"*

___

###  SetSelectionOperation

Ƭ **SetSelectionOperation**: *object | object | object*

___

###  SplitNodeOperation

Ƭ **SplitNodeOperation**: *object*

#### Type declaration:

* \[ **key**: *string*\]: any

* **path**: *[Path](_interfaces_path_.md#path)*

* **position**: *number*

* **properties**: *Partial‹[Node](_interfaces_node_.md#node)›*

* **target**: *number | null*

* **type**: *"split_node"*

___

###  TextOperation

Ƭ **TextOperation**: *[InsertTextOperation](_interfaces_operation_.md#inserttextoperation) | [RemoveTextOperation](_interfaces_operation_.md#removetextoperation)*

## Object literals

### `Const` Operation

### ▪ **Operation**: *object*

###  inverse

▸ **inverse**(`op`: [Operation](_interfaces_operation_.md#operation)): *[Operation](_interfaces_operation_.md#operation)*

Invert an operation, returning a new operation that will exactly undo the
original when applied.

**Parameters:**

Name | Type |
------ | ------ |
`op` | [Operation](_interfaces_operation_.md#operation) |

**Returns:** *[Operation](_interfaces_operation_.md#operation)*

###  isNodeOperation

▸ **isNodeOperation**(`value`: any): *value is NodeOperation*

Check of a value is a `NodeOperation` object.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is NodeOperation*

###  isOperation

▸ **isOperation**(`value`: any): *value is Operation*

Check of a value is an `Operation` object.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is Operation*

###  isOperationList

▸ **isOperationList**(`value`: any): *value is Operation[]*

Check if a value is a list of `Operation` objects.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is Operation[]*

###  isSelectionOperation

▸ **isSelectionOperation**(`value`: any): *value is SelectionOperation*

Check of a value is a `SelectionOperation` object.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is SelectionOperation*

###  isTextOperation

▸ **isTextOperation**(`value`: any): *value is TextOperation*

Check of a value is a `TextOperation` object.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is TextOperation*
