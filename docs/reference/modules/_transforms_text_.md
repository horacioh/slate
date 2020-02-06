
# External module: "transforms/text"

## Index

### Object literals

* [TextTransforms](_transforms_text_.md#const-texttransforms)

## Object literals

### `Const` TextTransforms

### ▪ **TextTransforms**: *object*

###  delete

▸ **delete**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *void*

Delete content in the editor.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) |
`distance?` | number |
`hanging?` | boolean |
`reverse?` | boolean |
`unit?` | "character" &#124; "word" &#124; "line" &#124; "block" |
`voids?` | boolean |

**Returns:** *void*

###  insertFragment

▸ **insertFragment**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `fragment`: [Node](_interfaces_node_.md#node)[], `options`: object): *void*

Insert a fragment at a specific location in the editor.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **fragment**: *[Node](_interfaces_node_.md#node)[]*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) |
`hanging?` | boolean |
`voids?` | boolean |

**Returns:** *void*

###  insertText

▸ **insertText**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `text`: string, `options`: object): *void*

Insert a string of text in the Editor.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **text**: *string*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) |
`voids?` | boolean |

**Returns:** *void*
