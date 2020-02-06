[slate](../README.md) › [Globals](../globals.md) › ["interfaces/editor"](_interfaces_editor_.md)

# External module: "interfaces/editor"

## Index

### Interfaces

* [Editor](../interfaces/_interfaces_editor_.editor.md)

### Type aliases

* [NodeMatch](_interfaces_editor_.md#nodematch)

### Object literals

* [Editor](_interfaces_editor_.md#const-editor)

## Type aliases

###  NodeMatch

Ƭ **NodeMatch**: *function | function*

*Defined in [interfaces/editor.ts:1596](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L1596)*

A helper type for narrowing matched nodes with a predicate.

## Object literals

### `Const` Editor

### ▪ **Editor**: *object*

*Defined in [interfaces/editor.ts:62](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L62)*

###  above

▸ **above**<**T**>(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *[NodeEntry](_interfaces_node_.md#nodeentry)‹T› | undefined*

*Defined in [interfaces/editor.ts:67](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L67)*

Get the ancestor above a location in the document.

**Type parameters:**

▪ **T**: *[Ancestor](_interfaces_node_.md#ancestor)*

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) |
`match?` | [NodeMatch](_interfaces_editor_.md#nodematch)‹T› |
`mode?` | "highest" &#124; "lowest" |
`voids?` | boolean |

**Returns:** *[NodeEntry](_interfaces_node_.md#nodeentry)‹T› | undefined*

###  addMark

▸ **addMark**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `key`: string, `value`: any): *void*

*Defined in [interfaces/editor.ts:109](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L109)*

Add a custom property to the leaf text nodes in the current selection.

If the selection is currently collapsed, the marks will be added to the
`editor.marks` property instead, and applied when text is inserted next.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`key` | string |
`value` | any |

**Returns:** *void*

###  after

▸ **after**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `at`: [Location](_interfaces_location_.md#location), `options`: object): *[Point](../interfaces/_interfaces_point_.point.md) | undefined*

*Defined in [interfaces/editor.ts:117](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L117)*

Get the point after a location.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **at**: *[Location](_interfaces_location_.md#location)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`distance?` | number |
`unit?` | "offset" &#124; "character" &#124; "word" &#124; "line" &#124; "block" |

**Returns:** *[Point](../interfaces/_interfaces_point_.point.md) | undefined*

###  before

▸ **before**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `at`: [Location](_interfaces_location_.md#location), `options`: object): *[Point](../interfaces/_interfaces_point_.point.md) | undefined*

*Defined in [interfaces/editor.ts:151](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L151)*

Get the point before a location.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **at**: *[Location](_interfaces_location_.md#location)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`distance?` | number |
`unit?` | "offset" &#124; "character" &#124; "word" &#124; "line" &#124; "block" |

**Returns:** *[Point](../interfaces/_interfaces_point_.point.md) | undefined*

###  deleteBackward

▸ **deleteBackward**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *void*

*Defined in [interfaces/editor.ts:189](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L189)*

Delete content in the editor backward from the current selection.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`unit?` | "character" &#124; "word" &#124; "line" &#124; "block" |

**Returns:** *void*

###  deleteForward

▸ **deleteForward**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *void*

*Defined in [interfaces/editor.ts:203](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L203)*

Delete content in the editor forward from the current selection.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`unit?` | "character" &#124; "word" &#124; "line" &#124; "block" |

**Returns:** *void*

###  deleteFragment

▸ **deleteFragment**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md)): *void*

*Defined in [interfaces/editor.ts:217](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L217)*

Delete the content in the current selection.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |

**Returns:** *void*

###  edges

▸ **edges**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `at`: [Location](_interfaces_location_.md#location)): *[[Point](../interfaces/_interfaces_point_.point.md), [Point](../interfaces/_interfaces_point_.point.md)]*

*Defined in [interfaces/editor.ts:225](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L225)*

Get the start and end points of a location.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`at` | [Location](_interfaces_location_.md#location) |

**Returns:** *[[Point](../interfaces/_interfaces_point_.point.md), [Point](../interfaces/_interfaces_point_.point.md)]*

###  end

▸ **end**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `at`: [Location](_interfaces_location_.md#location)): *[Point](../interfaces/_interfaces_point_.point.md)*

*Defined in [interfaces/editor.ts:233](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L233)*

Get the end point of a location.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`at` | [Location](_interfaces_location_.md#location) |

**Returns:** *[Point](../interfaces/_interfaces_point_.point.md)*

###  first

▸ **first**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `at`: [Location](_interfaces_location_.md#location)): *[NodeEntry](_interfaces_node_.md#nodeentry)*

*Defined in [interfaces/editor.ts:241](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L241)*

Get the first node at a location.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`at` | [Location](_interfaces_location_.md#location) |

**Returns:** *[NodeEntry](_interfaces_node_.md#nodeentry)*

###  fragment

▸ **fragment**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `at`: [Location](_interfaces_location_.md#location)): *[Descendant](_interfaces_node_.md#descendant)[]*

*Defined in [interfaces/editor.ts:250](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L250)*

Get the fragment at a location.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`at` | [Location](_interfaces_location_.md#location) |

**Returns:** *[Descendant](_interfaces_node_.md#descendant)[]*

###  hasBlocks

▸ **hasBlocks**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `element`: [Element](../interfaces/_interfaces_element_.element.md)): *boolean*

*Defined in [interfaces/editor.ts:259](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L259)*

Check if a node has block children.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`element` | [Element](../interfaces/_interfaces_element_.element.md) |

**Returns:** *boolean*

###  hasInlines

▸ **hasInlines**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `element`: [Element](../interfaces/_interfaces_element_.element.md)): *boolean*

*Defined in [interfaces/editor.ts:267](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L267)*

Check if a node has inline and text children.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`element` | [Element](../interfaces/_interfaces_element_.element.md) |

**Returns:** *boolean*

###  hasTexts

▸ **hasTexts**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `element`: [Element](../interfaces/_interfaces_element_.element.md)): *boolean*

*Defined in [interfaces/editor.ts:277](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L277)*

Check if a node has text children.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`element` | [Element](../interfaces/_interfaces_element_.element.md) |

**Returns:** *boolean*

###  insertBreak

▸ **insertBreak**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md)): *void*

*Defined in [interfaces/editor.ts:287](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L287)*

Insert a block break at the current selection.

If the selection is currently expanded, it will be deleted first.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |

**Returns:** *void*

###  insertFragment

▸ **insertFragment**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `fragment`: [Node](_interfaces_node_.md#node)[]): *void*

*Defined in [interfaces/editor.ts:297](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L297)*

Insert a fragment at the current selection.

If the selection is currently expanded, it will be deleted first.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`fragment` | [Node](_interfaces_node_.md#node)[] |

**Returns:** *void*

###  insertNode

▸ **insertNode**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `node`: [Node](_interfaces_node_.md#node)): *void*

*Defined in [interfaces/editor.ts:307](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L307)*

Insert a node at the current selection.

If the selection is currently expanded, it will be deleted first.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`node` | [Node](_interfaces_node_.md#node) |

**Returns:** *void*

###  insertText

▸ **insertText**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `text`: string): *void*

*Defined in [interfaces/editor.ts:317](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L317)*

Insert text at the current selection.

If the selection is currently expanded, it will be deleted first.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`text` | string |

**Returns:** *void*

###  isBlock

▸ **isBlock**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `value`: any): *value is Element*

*Defined in [interfaces/editor.ts:325](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L325)*

Check if a value is a block `Element` object.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`value` | any |

**Returns:** *value is Element*

###  isEdge

▸ **isEdge**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `point`: [Point](../interfaces/_interfaces_point_.point.md), `at`: [Location](_interfaces_location_.md#location)): *boolean*

*Defined in [interfaces/editor.ts:370](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L370)*

Check if a point is an edge of a location.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`point` | [Point](../interfaces/_interfaces_point_.point.md) |
`at` | [Location](_interfaces_location_.md#location) |

**Returns:** *boolean*

###  isEditor

▸ **isEditor**(`value`: any): *value is Editor*

*Defined in [interfaces/editor.ts:333](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L333)*

Check if a value is an `Editor` object.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is Editor*

###  isEmpty

▸ **isEmpty**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `element`: [Element](../interfaces/_interfaces_element_.element.md)): *boolean*

*Defined in [interfaces/editor.ts:378](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L378)*

Check if an element is empty, accounting for void nodes.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`element` | [Element](../interfaces/_interfaces_element_.element.md) |

**Returns:** *boolean*

###  isEnd

▸ **isEnd**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `point`: [Point](../interfaces/_interfaces_point_.point.md), `at`: [Location](_interfaces_location_.md#location)): *boolean*

*Defined in [interfaces/editor.ts:361](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L361)*

Check if a point is the end point of a location.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`point` | [Point](../interfaces/_interfaces_point_.point.md) |
`at` | [Location](_interfaces_location_.md#location) |

**Returns:** *boolean*

###  isInline

▸ **isInline**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `value`: any): *value is Element*

*Defined in [interfaces/editor.ts:394](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L394)*

Check if a value is an inline `Element` object.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`value` | any |

**Returns:** *value is Element*

###  isNormalizing

▸ **isNormalizing**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md)): *boolean*

*Defined in [interfaces/editor.ts:402](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L402)*

Check if the editor is currently normalizing after each operation.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |

**Returns:** *boolean*

###  isStart

▸ **isStart**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `point`: [Point](../interfaces/_interfaces_point_.point.md), `at`: [Location](_interfaces_location_.md#location)): *boolean*

*Defined in [interfaces/editor.ts:411](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L411)*

Check if a point is the start point of a location.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`point` | [Point](../interfaces/_interfaces_point_.point.md) |
`at` | [Location](_interfaces_location_.md#location) |

**Returns:** *boolean*

###  isVoid

▸ **isVoid**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `value`: any): *value is Element*

*Defined in [interfaces/editor.ts:425](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L425)*

Check if a value is a void `Element` object.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`value` | any |

**Returns:** *value is Element*

###  last

▸ **last**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `at`: [Location](_interfaces_location_.md#location)): *[NodeEntry](_interfaces_node_.md#nodeentry)*

*Defined in [interfaces/editor.ts:433](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L433)*

Get the last node at a location.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`at` | [Location](_interfaces_location_.md#location) |

**Returns:** *[NodeEntry](_interfaces_node_.md#nodeentry)*

###  leaf

▸ **leaf**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `at`: [Location](_interfaces_location_.md#location), `options`: object): *[NodeEntry](_interfaces_node_.md#nodeentry)‹[Text](../interfaces/_interfaces_text_.text.md)›*

*Defined in [interfaces/editor.ts:442](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L442)*

Get the leaf text node at a location.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **at**: *[Location](_interfaces_location_.md#location)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`depth?` | number |
`edge?` | "start" &#124; "end" |

**Returns:** *[NodeEntry](_interfaces_node_.md#nodeentry)‹[Text](../interfaces/_interfaces_text_.text.md)›*

###  levels

▸ **levels**<**T**>(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *Iterable‹[NodeEntry](_interfaces_node_.md#nodeentry)‹T››*

*Defined in [interfaces/editor.ts:459](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L459)*

Iterate through all of the levels at a location.

**Type parameters:**

▪ **T**: *[Node](_interfaces_node_.md#node)*

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) |
`match?` | [NodeMatch](_interfaces_editor_.md#nodematch)‹T› |
`reverse?` | boolean |
`voids?` | boolean |

**Returns:** *Iterable‹[NodeEntry](_interfaces_node_.md#nodeentry)‹T››*

###  marks

▸ **marks**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md)): *Record‹string, any› | null*

*Defined in [interfaces/editor.ts:505](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L505)*

Get the marks that would be added to text at the current selection.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |

**Returns:** *Record‹string, any› | null*

###  next

▸ **next**<**T**>(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *[NodeEntry](_interfaces_node_.md#nodeentry)‹T› | undefined*

*Defined in [interfaces/editor.ts:556](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L556)*

Get the matching node in the branch of the document after a location.

**Type parameters:**

▪ **T**: *[Node](_interfaces_node_.md#node)*

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) |
`match?` | [NodeMatch](_interfaces_editor_.md#nodematch)‹T› |
`mode?` | "all" &#124; "highest" &#124; "lowest" |
`voids?` | boolean |

**Returns:** *[NodeEntry](_interfaces_node_.md#nodeentry)‹T› | undefined*

###  node

▸ **node**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `at`: [Location](_interfaces_location_.md#location), `options`: object): *[NodeEntry](_interfaces_node_.md#nodeentry)*

*Defined in [interfaces/editor.ts:597](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L597)*

Get the node at a location.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **at**: *[Location](_interfaces_location_.md#location)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`depth?` | number |
`edge?` | "start" &#124; "end" |

**Returns:** *[NodeEntry](_interfaces_node_.md#nodeentry)*

###  nodes

▸ **nodes**<**T**>(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *Iterable‹[NodeEntry](_interfaces_node_.md#nodeentry)‹T››*

*Defined in [interfaces/editor.ts:614](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L614)*

Iterate through all of the nodes in the Editor.

**Type parameters:**

▪ **T**: *[Node](_interfaces_node_.md#node)*

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) &#124; [Span](_interfaces_location_.md#span) |
`match?` | [NodeMatch](_interfaces_editor_.md#nodematch)‹T› |
`mode?` | "all" &#124; "highest" &#124; "lowest" |
`reverse?` | boolean |
`universal?` | boolean |
`voids?` | boolean |

**Returns:** *Iterable‹[NodeEntry](_interfaces_node_.md#nodeentry)‹T››*

###  normalize

▸ **normalize**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *void*

*Defined in [interfaces/editor.ts:724](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L724)*

Normalize any dirty objects in the editor.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`force?` | boolean |

**Returns:** *void*

###  parent

▸ **parent**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `at`: [Location](_interfaces_location_.md#location), `options`: object): *[NodeEntry](_interfaces_node_.md#nodeentry)‹[Ancestor](_interfaces_node_.md#ancestor)›*

*Defined in [interfaces/editor.ts:771](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L771)*

Get the parent node of a location.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **at**: *[Location](_interfaces_location_.md#location)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`depth?` | number |
`edge?` | "start" &#124; "end" |

**Returns:** *[NodeEntry](_interfaces_node_.md#nodeentry)‹[Ancestor](_interfaces_node_.md#ancestor)›*

###  path

▸ **path**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `at`: [Location](_interfaces_location_.md#location), `options`: object): *[Path](_interfaces_path_.md#path)*

*Defined in [interfaces/editor.ts:789](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L789)*

Get the path of a location.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **at**: *[Location](_interfaces_location_.md#location)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`depth?` | number |
`edge?` | "start" &#124; "end" |

**Returns:** *[Path](_interfaces_path_.md#path)*

###  pathRef

▸ **pathRef**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `path`: [Path](_interfaces_path_.md#path), `options`: object): *[PathRef](../interfaces/_interfaces_path_ref_.pathref.md)*

*Defined in [interfaces/editor.ts:835](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L835)*

Create a mutable ref for a `Path` object, which will stay in sync as new
operations are applied to the editor.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **path**: *[Path](_interfaces_path_.md#path)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`affinity?` | "backward" &#124; "forward" &#124; null |

**Returns:** *[PathRef](../interfaces/_interfaces_path_ref_.pathref.md)*

###  pathRefs

▸ **pathRefs**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md)): *Set‹[PathRef](../interfaces/_interfaces_path_ref_.pathref.md)›*

*Defined in [interfaces/editor.ts:864](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L864)*

Get the set of currently tracked path refs of the editor.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |

**Returns:** *Set‹[PathRef](../interfaces/_interfaces_path_ref_.pathref.md)›*

###  point

▸ **point**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `at`: [Location](_interfaces_location_.md#location), `options`: object): *[Point](../interfaces/_interfaces_point_.point.md)*

*Defined in [interfaces/editor.ts:879](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L879)*

Get the start or end point of a location.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **at**: *[Location](_interfaces_location_.md#location)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`edge?` | "start" &#124; "end" |

**Returns:** *[Point](../interfaces/_interfaces_point_.point.md)*

###  pointRef

▸ **pointRef**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `point`: [Point](../interfaces/_interfaces_point_.point.md), `options`: object): *[PointRef](../interfaces/_interfaces_point_ref_.pointref.md)*

*Defined in [interfaces/editor.ts:923](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L923)*

Create a mutable ref for a `Point` object, which will stay in sync as new
operations are applied to the editor.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **point**: *[Point](../interfaces/_interfaces_point_.point.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`affinity?` | "backward" &#124; "forward" &#124; null |

**Returns:** *[PointRef](../interfaces/_interfaces_point_ref_.pointref.md)*

###  pointRefs

▸ **pointRefs**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md)): *Set‹[PointRef](../interfaces/_interfaces_point_ref_.pointref.md)›*

*Defined in [interfaces/editor.ts:952](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L952)*

Get the set of currently tracked point refs of the editor.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |

**Returns:** *Set‹[PointRef](../interfaces/_interfaces_point_ref_.pointref.md)›*

###  positions

▸ **positions**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *Iterable‹[Point](../interfaces/_interfaces_point_.point.md)›*

*Defined in [interfaces/editor.ts:975](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L975)*

Iterate through all of the positions in the document where a `Point` can be
placed.

By default it will move forward by individual offsets at a time,  but you
can pass the `unit: 'character'` option to moved forward one character, word,
or line at at time.

Note: void nodes are treated as a single point, and iteration will not
happen inside their content.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) |
`reverse?` | boolean |
`unit?` | "offset" &#124; "character" &#124; "word" &#124; "line" &#124; "block" |

**Returns:** *Iterable‹[Point](../interfaces/_interfaces_point_.point.md)›*

###  previous

▸ **previous**<**T**>(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *[NodeEntry](_interfaces_node_.md#nodeentry)‹T› | undefined*

*Defined in [interfaces/editor.ts:1089](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L1089)*

Get the matching node in the branch of the document before a location.

**Type parameters:**

▪ **T**: *[Node](_interfaces_node_.md#node)*

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) |
`match?` | [NodeMatch](_interfaces_editor_.md#nodematch)‹T› |
`mode?` | "all" &#124; "highest" &#124; "lowest" |
`voids?` | boolean |

**Returns:** *[NodeEntry](_interfaces_node_.md#nodeentry)‹T› | undefined*

###  range

▸ **range**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `at`: [Location](_interfaces_location_.md#location), `to?`: [Location](_interfaces_location_.md#location)): *[Range](../interfaces/_interfaces_range_.range.md)*

*Defined in [interfaces/editor.ts:1137](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L1137)*

Get a range of a location.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`at` | [Location](_interfaces_location_.md#location) |
`to?` | [Location](_interfaces_location_.md#location) |

**Returns:** *[Range](../interfaces/_interfaces_range_.range.md)*

###  rangeRef

▸ **rangeRef**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `range`: [Range](../interfaces/_interfaces_range_.range.md), `options`: object): *[RangeRef](../interfaces/_interfaces_range_ref_.rangeref.md)*

*Defined in [interfaces/editor.ts:1152](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L1152)*

Create a mutable ref for a `Range` object, which will stay in sync as new
operations are applied to the editor.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **range**: *[Range](../interfaces/_interfaces_range_.range.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`affinity?` | "backward" &#124; "forward" &#124; "outward" &#124; "inward" &#124; null |

**Returns:** *[RangeRef](../interfaces/_interfaces_range_ref_.rangeref.md)*

###  rangeRefs

▸ **rangeRefs**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md)): *Set‹[RangeRef](../interfaces/_interfaces_range_ref_.rangeref.md)›*

*Defined in [interfaces/editor.ts:1181](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L1181)*

Get the set of currently tracked range refs of the editor.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |

**Returns:** *Set‹[RangeRef](../interfaces/_interfaces_range_ref_.rangeref.md)›*

###  removeMark

▸ **removeMark**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `key`: string): *void*

*Defined in [interfaces/editor.ts:1200](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L1200)*

Remove a custom property from all of the leaf text nodes in the current
selection.

If the selection is currently collapsed, the removal will be stored on
`editor.marks` and applied to the text inserted next.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`key` | string |

**Returns:** *void*

###  start

▸ **start**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `at`: [Location](_interfaces_location_.md#location)): *[Point](../interfaces/_interfaces_point_.point.md)*

*Defined in [interfaces/editor.ts:1208](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L1208)*

Get the start point of a location.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`at` | [Location](_interfaces_location_.md#location) |

**Returns:** *[Point](../interfaces/_interfaces_point_.point.md)*

###  string

▸ **string**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `at`: [Location](_interfaces_location_.md#location)): *string*

*Defined in [interfaces/editor.ts:1219](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L1219)*

Get the text string content of a location.

Note: the text of void nodes is presumed to be an empty string, regardless
of what their actual content is.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`at` | [Location](_interfaces_location_.md#location) |

**Returns:** *string*

###  transform

▸ **transform**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `op`: [Operation](_interfaces_operation_.md#operation)): *void*

*Defined in [interfaces/editor.ts:1248](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L1248)*

Transform the editor by an operation.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`op` | [Operation](_interfaces_operation_.md#operation) |

**Returns:** *void*

###  unhangRange

▸ **unhangRange**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `range`: [Range](../interfaces/_interfaces_range_.range.md), `options`: object): *[Range](../interfaces/_interfaces_range_.range.md)*

*Defined in [interfaces/editor.ts:1517](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L1517)*

Convert a range into a non-hanging one.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **range**: *[Range](../interfaces/_interfaces_range_.range.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`voids?` | boolean |

**Returns:** *[Range](../interfaces/_interfaces_range_.range.md)*

###  void

▸ **void**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *[NodeEntry](_interfaces_node_.md#nodeentry)‹[Element](../interfaces/_interfaces_element_.element.md)› | undefined*

*Defined in [interfaces/editor.ts:1565](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L1565)*

Match a void node in the current branch of the editor.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) |
`mode?` | "highest" &#124; "lowest" |
`voids?` | boolean |

**Returns:** *[NodeEntry](_interfaces_node_.md#nodeentry)‹[Element](../interfaces/_interfaces_element_.element.md)› | undefined*

###  withoutNormalizing

▸ **withoutNormalizing**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `fn`: function): *void*

*Defined in [interfaces/editor.ts:1583](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L1583)*

Call a function, deferring normalization until after it completes.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **fn**: *function*

▸ (): *void*

**Returns:** *void*
