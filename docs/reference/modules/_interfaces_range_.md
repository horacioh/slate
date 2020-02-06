[slate](../README.md) › [Globals](../globals.md) › ["interfaces/range"](_interfaces_range_.md)

# External module: "interfaces/range"

## Index

### Interfaces

* [Range](../interfaces/_interfaces_range_.range.md)

### Object literals

* [Range](_interfaces_range_.md#const-range)

## Object literals

### `Const` Range

### ▪ **Range**: *object*

*Defined in [interfaces/range.ts:17](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/range.ts#L17)*

###  edges

▸ **edges**(`range`: [Range](../interfaces/_interfaces_range_.range.md), `options`: object): *[[Point](../interfaces/_interfaces_point_.point.md), [Point](../interfaces/_interfaces_point_.point.md)]*

*Defined in [interfaces/range.ts:23](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/range.ts#L23)*

Get the start and end points of a range, in the order in which they appear
in the document.

**Parameters:**

▪ **range**: *[Range](../interfaces/_interfaces_range_.range.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`reverse?` | boolean |

**Returns:** *[[Point](../interfaces/_interfaces_point_.point.md), [Point](../interfaces/_interfaces_point_.point.md)]*

###  end

▸ **end**(`range`: [Range](../interfaces/_interfaces_range_.range.md)): *[Point](../interfaces/_interfaces_point_.point.md)*

*Defined in [interfaces/range.ts:40](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/range.ts#L40)*

Get the end point of a range.

**Parameters:**

Name | Type |
------ | ------ |
`range` | [Range](../interfaces/_interfaces_range_.range.md) |

**Returns:** *[Point](../interfaces/_interfaces_point_.point.md)*

###  equals

▸ **equals**(`range`: [Range](../interfaces/_interfaces_range_.range.md), `another`: [Range](../interfaces/_interfaces_range_.range.md)): *boolean*

*Defined in [interfaces/range.ts:49](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/range.ts#L49)*

Check if a range is exactly equal to another.

**Parameters:**

Name | Type |
------ | ------ |
`range` | [Range](../interfaces/_interfaces_range_.range.md) |
`another` | [Range](../interfaces/_interfaces_range_.range.md) |

**Returns:** *boolean*

###  includes

▸ **includes**(`range`: [Range](../interfaces/_interfaces_range_.range.md), `target`: [Path](_interfaces_path_.md#path) | [Point](../interfaces/_interfaces_point_.point.md) | [Range](../interfaces/_interfaces_range_.range.md)): *boolean*

*Defined in [interfaces/range.ts:60](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/range.ts#L60)*

Check if a range includes a path, a point or part of another range.

**Parameters:**

Name | Type |
------ | ------ |
`range` | [Range](../interfaces/_interfaces_range_.range.md) |
`target` | [Path](_interfaces_path_.md#path) &#124; [Point](../interfaces/_interfaces_point_.point.md) &#124; [Range](../interfaces/_interfaces_range_.range.md) |

**Returns:** *boolean*

###  intersection

▸ **intersection**(`range`: [Range](../interfaces/_interfaces_range_.range.md), `another`: [Range](../interfaces/_interfaces_range_.range.md)): *[Range](../interfaces/_interfaces_range_.range.md) | null*

*Defined in [interfaces/range.ts:93](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/range.ts#L93)*

Get the intersection of a range with another.

**Parameters:**

Name | Type |
------ | ------ |
`range` | [Range](../interfaces/_interfaces_range_.range.md) |
`another` | [Range](../interfaces/_interfaces_range_.range.md) |

**Returns:** *[Range](../interfaces/_interfaces_range_.range.md) | null*

###  isBackward

▸ **isBackward**(`range`: [Range](../interfaces/_interfaces_range_.range.md)): *boolean*

*Defined in [interfaces/range.ts:112](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/range.ts#L112)*

Check if a range is backward, meaning that its anchor point appears in the
document _after_ its focus point.

**Parameters:**

Name | Type |
------ | ------ |
`range` | [Range](../interfaces/_interfaces_range_.range.md) |

**Returns:** *boolean*

###  isCollapsed

▸ **isCollapsed**(`range`: [Range](../interfaces/_interfaces_range_.range.md)): *boolean*

*Defined in [interfaces/range.ts:122](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/range.ts#L122)*

Check if a range is collapsed, meaning that both its anchor and focus
points refer to the exact same position in the document.

**Parameters:**

Name | Type |
------ | ------ |
`range` | [Range](../interfaces/_interfaces_range_.range.md) |

**Returns:** *boolean*

###  isExpanded

▸ **isExpanded**(`range`: [Range](../interfaces/_interfaces_range_.range.md)): *boolean*

*Defined in [interfaces/range.ts:133](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/range.ts#L133)*

Check if a range is expanded.

This is the opposite of [Range.isCollapsed](_interfaces_range_.md#iscollapsed) and is provided for legibility.

**Parameters:**

Name | Type |
------ | ------ |
`range` | [Range](../interfaces/_interfaces_range_.range.md) |

**Returns:** *boolean*

###  isForward

▸ **isForward**(`range`: [Range](../interfaces/_interfaces_range_.range.md)): *boolean*

*Defined in [interfaces/range.ts:143](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/range.ts#L143)*

Check if a range is forward.

This is the opposite of [Range.isBackward](_interfaces_range_.md#isbackward) and is provided for legibility.

**Parameters:**

Name | Type |
------ | ------ |
`range` | [Range](../interfaces/_interfaces_range_.range.md) |

**Returns:** *boolean*

###  isRange

▸ **isRange**(`value`: any): *value is Range*

*Defined in [interfaces/range.ts:151](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/range.ts#L151)*

Check if a value implements the [Range](../interfaces/_interfaces_range_.range.md) interface.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is Range*

###  points

▸ **points**(`range`: [Range](../interfaces/_interfaces_range_.range.md)): *Iterable‹[PointEntry](_interfaces_point_.md#pointentry)›*

*Defined in [interfaces/range.ts:163](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/range.ts#L163)*

Iterate through all of the point entries in a range.

**Parameters:**

Name | Type |
------ | ------ |
`range` | [Range](../interfaces/_interfaces_range_.range.md) |

**Returns:** *Iterable‹[PointEntry](_interfaces_point_.md#pointentry)›*

###  start

▸ **start**(`range`: [Range](../interfaces/_interfaces_range_.range.md)): *[Point](../interfaces/_interfaces_point_.point.md)*

*Defined in [interfaces/range.ts:172](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/range.ts#L172)*

Get the start point of a range.

**Parameters:**

Name | Type |
------ | ------ |
`range` | [Range](../interfaces/_interfaces_range_.range.md) |

**Returns:** *[Point](../interfaces/_interfaces_point_.point.md)*

###  transform

▸ **transform**(`range`: [Range](../interfaces/_interfaces_range_.range.md), `op`: [Operation](_interfaces_operation_.md#operation), `options`: object): *[Range](../interfaces/_interfaces_range_.range.md) | null*

*Defined in [interfaces/range.ts:181](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/range.ts#L181)*

Transform a range by an operation.

**Parameters:**

▪ **range**: *[Range](../interfaces/_interfaces_range_.range.md)*

▪ **op**: *[Operation](_interfaces_operation_.md#operation)*

▪ **options**: *object*

Name | Type |
------ | ------ |
`affinity` | "forward" &#124; "backward" &#124; "outward" &#124; "inward" &#124; null |

**Returns:** *[Range](../interfaces/_interfaces_range_.range.md) | null*
