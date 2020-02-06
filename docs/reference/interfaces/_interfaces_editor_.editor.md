[slate](../README.md) › [Globals](../globals.md) › ["interfaces/editor"](../modules/_interfaces_editor_.md) › [Editor](_interfaces_editor_.editor.md)

# Interface: Editor

The `Editor` interface stores all the state of a Slate editor. It is extended
by plugins that wish to add their own helpers and implement new behaviors.

## Hierarchy

* **Editor**

## Indexable

* \[ **key**: *string*\]: any

The `Editor` interface stores all the state of a Slate editor. It is extended
by plugins that wish to add their own helpers and implement new behaviors.

## Index

### Properties

* [addMark](_interfaces_editor_.editor.md#addmark)
* [apply](_interfaces_editor_.editor.md#apply)
* [children](_interfaces_editor_.editor.md#children)
* [deleteBackward](_interfaces_editor_.editor.md#deletebackward)
* [deleteForward](_interfaces_editor_.editor.md#deleteforward)
* [deleteFragment](_interfaces_editor_.editor.md#deletefragment)
* [insertBreak](_interfaces_editor_.editor.md#insertbreak)
* [insertFragment](_interfaces_editor_.editor.md#insertfragment)
* [insertNode](_interfaces_editor_.editor.md#insertnode)
* [insertText](_interfaces_editor_.editor.md#inserttext)
* [isInline](_interfaces_editor_.editor.md#isinline)
* [isVoid](_interfaces_editor_.editor.md#isvoid)
* [marks](_interfaces_editor_.editor.md#marks)
* [normalizeNode](_interfaces_editor_.editor.md#normalizenode)
* [onChange](_interfaces_editor_.editor.md#onchange)
* [operations](_interfaces_editor_.editor.md#operations)
* [removeMark](_interfaces_editor_.editor.md#removemark)
* [selection](_interfaces_editor_.editor.md#selection)

## Properties

###  addMark

• **addMark**: *function*

*Defined in [interfaces/editor.ts:50](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L50)*

#### Type declaration:

▸ (`key`: string, `value`: any): *void*

**Parameters:**

Name | Type |
------ | ------ |
`key` | string |
`value` | any |

___

###  apply

• **apply**: *function*

*Defined in [interfaces/editor.ts:51](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L51)*

#### Type declaration:

▸ (`operation`: [Operation](../modules/_interfaces_operation_.md#operation)): *void*

**Parameters:**

Name | Type |
------ | ------ |
`operation` | [Operation](../modules/_interfaces_operation_.md#operation) |

___

###  children

• **children**: *[Node](../modules/_interfaces_node_.md#node)[]*

*Defined in [interfaces/editor.ts:37](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L37)*

___

###  deleteBackward

• **deleteBackward**: *function*

*Defined in [interfaces/editor.ts:52](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L52)*

#### Type declaration:

▸ (`unit`: "character" | "word" | "line" | "block"): *void*

**Parameters:**

Name | Type |
------ | ------ |
`unit` | "character" &#124; "word" &#124; "line" &#124; "block" |

___

###  deleteForward

• **deleteForward**: *function*

*Defined in [interfaces/editor.ts:53](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L53)*

#### Type declaration:

▸ (`unit`: "character" | "word" | "line" | "block"): *void*

**Parameters:**

Name | Type |
------ | ------ |
`unit` | "character" &#124; "word" &#124; "line" &#124; "block" |

___

###  deleteFragment

• **deleteFragment**: *function*

*Defined in [interfaces/editor.ts:54](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L54)*

#### Type declaration:

▸ (): *void*

___

###  insertBreak

• **insertBreak**: *function*

*Defined in [interfaces/editor.ts:55](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L55)*

#### Type declaration:

▸ (): *void*

___

###  insertFragment

• **insertFragment**: *function*

*Defined in [interfaces/editor.ts:56](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L56)*

#### Type declaration:

▸ (`fragment`: [Node](../modules/_interfaces_node_.md#node)[]): *void*

**Parameters:**

Name | Type |
------ | ------ |
`fragment` | [Node](../modules/_interfaces_node_.md#node)[] |

___

###  insertNode

• **insertNode**: *function*

*Defined in [interfaces/editor.ts:57](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L57)*

#### Type declaration:

▸ (`node`: [Node](../modules/_interfaces_node_.md#node)): *void*

**Parameters:**

Name | Type |
------ | ------ |
`node` | [Node](../modules/_interfaces_node_.md#node) |

___

###  insertText

• **insertText**: *function*

*Defined in [interfaces/editor.ts:58](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L58)*

#### Type declaration:

▸ (`text`: string): *void*

**Parameters:**

Name | Type |
------ | ------ |
`text` | string |

___

###  isInline

• **isInline**: *function*

*Defined in [interfaces/editor.ts:44](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L44)*

#### Type declaration:

▸ (`element`: [Element](_interfaces_element_.element.md)): *boolean*

**Parameters:**

Name | Type |
------ | ------ |
`element` | [Element](_interfaces_element_.element.md) |

___

###  isVoid

• **isVoid**: *function*

*Defined in [interfaces/editor.ts:45](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L45)*

#### Type declaration:

▸ (`element`: [Element](_interfaces_element_.element.md)): *boolean*

**Parameters:**

Name | Type |
------ | ------ |
`element` | [Element](_interfaces_element_.element.md) |

___

###  marks

• **marks**: *Record‹string, any› | null*

*Defined in [interfaces/editor.ts:40](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L40)*

___

###  normalizeNode

• **normalizeNode**: *function*

*Defined in [interfaces/editor.ts:46](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L46)*

#### Type declaration:

▸ (`entry`: [NodeEntry](../modules/_interfaces_node_.md#nodeentry)): *void*

**Parameters:**

Name | Type |
------ | ------ |
`entry` | [NodeEntry](../modules/_interfaces_node_.md#nodeentry) |

___

###  onChange

• **onChange**: *function*

*Defined in [interfaces/editor.ts:47](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L47)*

#### Type declaration:

▸ (): *void*

___

###  operations

• **operations**: *[Operation](../modules/_interfaces_operation_.md#operation)[]*

*Defined in [interfaces/editor.ts:39](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L39)*

___

###  removeMark

• **removeMark**: *function*

*Defined in [interfaces/editor.ts:59](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L59)*

#### Type declaration:

▸ (`key`: string): *void*

**Parameters:**

Name | Type |
------ | ------ |
`key` | string |

___

###  selection

• **selection**: *[Range](_interfaces_range_.range.md) | null*

*Defined in [interfaces/editor.ts:38](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/editor.ts#L38)*
