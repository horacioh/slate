[slate](../README.md) › [Globals](../globals.md) › ["transforms/selection"](_transforms_selection_.md)

# External module: "transforms/selection"

## Index

### Object literals

* [SelectionTransforms](_transforms_selection_.md#const-selectiontransforms)

## Object literals

### `Const` SelectionTransforms

### ▪ **SelectionTransforms**: *object*

*Defined in [transforms/selection.ts:3](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/selection.ts#L3)*

###  collapse

▸ **collapse**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *void*

*Defined in [transforms/selection.ts:8](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/selection.ts#L8)*

Collapse the selection.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`edge?` | "anchor" &#124; "focus" &#124; "start" &#124; "end" |

**Returns:** *void*

###  deselect

▸ **deselect**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md)): *void*

*Defined in [transforms/selection.ts:36](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/selection.ts#L36)*

Unset the selection.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |

**Returns:** *void*

###  move

▸ **move**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *void*

*Defined in [transforms/selection.ts:52](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/selection.ts#L52)*

Move the selection's point forward or backward.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`distance?` | number |
`edge?` | "anchor" &#124; "focus" &#124; "start" &#124; "end" |
`reverse?` | boolean |
`unit?` | "offset" &#124; "character" &#124; "word" &#124; "line" |

**Returns:** *void*

###  select

▸ **select**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `target`: [Location](_interfaces_location_.md#location)): *void*

*Defined in [transforms/selection.ts:108](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/selection.ts#L108)*

Set the selection to a new value.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`target` | [Location](_interfaces_location_.md#location) |

**Returns:** *void*

###  setPoint

▸ **setPoint**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `props`: Partial‹[Point](../interfaces/_interfaces_point_.point.md)›, `options`: object): *void*

*Defined in [transforms/selection.ts:136](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/selection.ts#L136)*

Set new properties on one of the selection's points.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **props**: *Partial‹[Point](../interfaces/_interfaces_point_.point.md)›*

▪ **options**: *object*

Name | Type |
------ | ------ |
`edge?` | "anchor" &#124; "focus" &#124; "start" &#124; "end" |

**Returns:** *void*

###  setSelection

▸ **setSelection**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `props`: Partial‹[Range](../interfaces/_interfaces_range_.range.md)›): *void*

*Defined in [transforms/selection.ts:173](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/selection.ts#L173)*

Set new properties on the selection.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`props` | Partial‹[Range](../interfaces/_interfaces_range_.range.md)› |

**Returns:** *void*
