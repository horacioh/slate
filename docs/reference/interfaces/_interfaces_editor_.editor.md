# Interface: Editor

The `Editor` interface stores all the state of a Slate editor. It is extended
by plugins that wish to add their own helpers and implement new behaviors.

## Hierarchy

- **Editor**

## Indexable

- \[ **key**: _string_\]: any

The `Editor` interface stores all the state of a Slate editor. It is extended
by plugins that wish to add their own helpers and implement new behaviors.

## Index

### Properties

- [addMark](_interfaces_editor_.editor.md#addmark)
- [apply](_interfaces_editor_.editor.md#apply)
- [children](_interfaces_editor_.editor.md#children)
- [deleteBackward](_interfaces_editor_.editor.md#deletebackward)
- [deleteForward](_interfaces_editor_.editor.md#deleteforward)
- [deleteFragment](_interfaces_editor_.editor.md#deletefragment)
- [insertBreak](_interfaces_editor_.editor.md#insertbreak)
- [insertFragment](_interfaces_editor_.editor.md#insertfragment)
- [insertNode](_interfaces_editor_.editor.md#insertnode)
- [insertText](_interfaces_editor_.editor.md#inserttext)
- [isInline](_interfaces_editor_.editor.md#isinline)
- [isVoid](_interfaces_editor_.editor.md#isvoid)
- [marks](_interfaces_editor_.editor.md#marks)
- [normalizeNode](_interfaces_editor_.editor.md#normalizenode)
- [onChange](_interfaces_editor_.editor.md#onchange)
- [operations](_interfaces_editor_.editor.md#operations)
- [removeMark](_interfaces_editor_.editor.md#removemark)
- [selection](_interfaces_editor_.editor.md#selection)

## Properties

### addMark

• **addMark**: _function_

#### Type declaration:

▸ (`key`: string, `value`: any): _void_

**Parameters:**

| Name    | Type   |
| ------- | ------ |
| `key`   | string |
| `value` | any    |

---

### apply

• **apply**: _function_

#### Type declaration:

▸ (`operation`: [Operation](../modules/_interfaces_operation_.md#operation)): _void_

**Parameters:**

| Name        | Type                                                        |
| ----------- | ----------------------------------------------------------- |
| `operation` | [Operation](../modules/_interfaces_operation_.md#operation) |

---

### children

• **children**: _[Node](../modules/\_interfaces_node_.md#node)[]\_

---

### deleteBackward

• **deleteBackward**: _function_

#### Type declaration:

▸ (`unit`: "character" | "word" | "line" | "block"): _void_

**Parameters:**

| Name   | Type                                                   |
| ------ | ------------------------------------------------------ |
| `unit` | "character" &#124; "word" &#124; "line" &#124; "block" |

---

### deleteForward

• **deleteForward**: _function_

#### Type declaration:

▸ (`unit`: "character" | "word" | "line" | "block"): _void_

**Parameters:**

| Name   | Type                                                   |
| ------ | ------------------------------------------------------ |
| `unit` | "character" &#124; "word" &#124; "line" &#124; "block" |

---

### deleteFragment

• **deleteFragment**: _function_

#### Type declaration:

▸ (): _void_

---

### insertBreak

• **insertBreak**: _function_

#### Type declaration:

▸ (): _void_

---

### insertFragment

• **insertFragment**: _function_

#### Type declaration:

▸ (`fragment`: [Node](../modules/_interfaces_node_.md#node)[]): _void_

**Parameters:**

| Name       | Type                                           |
| ---------- | ---------------------------------------------- |
| `fragment` | [Node](../modules/_interfaces_node_.md#node)[] |

---

### insertNode

• **insertNode**: _function_

#### Type declaration:

▸ (`node`: [Node](../modules/_interfaces_node_.md#node)): _void_

**Parameters:**

| Name   | Type                                         |
| ------ | -------------------------------------------- |
| `node` | [Node](../modules/_interfaces_node_.md#node) |

---

### insertText

• **insertText**: _function_

#### Type declaration:

▸ (`text`: string): _void_

**Parameters:**

| Name   | Type   |
| ------ | ------ |
| `text` | string |

---

### isInline

• **isInline**: _function_

#### Type declaration:

▸ (`element`: [Element](_interfaces_element_.element.md)): _boolean_

**Parameters:**

| Name      | Type                                       |
| --------- | ------------------------------------------ |
| `element` | [Element](_interfaces_element_.element.md) |

---

### isVoid

• **isVoid**: _function_

#### Type declaration:

▸ (`element`: [Element](_interfaces_element_.element.md)): _boolean_

**Parameters:**

| Name      | Type                                       |
| --------- | ------------------------------------------ |
| `element` | [Element](_interfaces_element_.element.md) |

---

### marks

• **marks**: _Record‹string, any› | null_

---

### normalizeNode

• **normalizeNode**: _function_

#### Type declaration:

▸ (`entry`: [NodeEntry](../modules/_interfaces_node_.md#nodeentry)): _void_

**Parameters:**

| Name    | Type                                                   |
| ------- | ------------------------------------------------------ |
| `entry` | [NodeEntry](../modules/_interfaces_node_.md#nodeentry) |

---

### onChange

• **onChange**: _function_

#### Type declaration:

▸ (): _void_

---

### operations

• **operations**: _[Operation](../modules/\_interfaces_operation_.md#operation)[]\_

---

### removeMark

• **removeMark**: _function_

#### Type declaration:

▸ (`key`: string): _void_

**Parameters:**

| Name  | Type   |
| ----- | ------ |
| `key` | string |

---

### selection

• **selection**: _[Range](\_interfaces_range_.range.md) | null\_
