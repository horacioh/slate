
# External module: "transforms/selection"

## Index

### Object literals

* [SelectionTransforms](_transforms_selection_.md#const-selectiontransforms)

## Object literals

### `Const` SelectionTransforms

### ▪ **SelectionTransforms**: *object*

###  collapse

▸ **collapse**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *void*

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

Unset the selection.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |

**Returns:** *void*

###  move

▸ **move**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *void*

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

Set the selection to a new value.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`target` | [Location](_interfaces_location_.md#location) |

**Returns:** *void*

###  setPoint

▸ **setPoint**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `props`: Partial‹[Point](../interfaces/_interfaces_point_.point.md)›, `options`: object): *void*

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

Set new properties on the selection.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`props` | Partial‹[Range](../interfaces/_interfaces_range_.range.md)› |

**Returns:** *void*
