
# External module: "interfaces/point"

## Index

### Interfaces

* [Point](../interfaces/_interfaces_point_.point.md)

### Type aliases

* [PointEntry](_interfaces_point_.md#pointentry)

### Object literals

* [Point](_interfaces_point_.md#const-point)

## Type aliases

###  PointEntry

Ƭ **PointEntry**: *[[Point](../interfaces/_interfaces_point_.point.md), "anchor" | "focus"]*

`PointEntry` objects are returned when iterating over `Point` objects that
belong to a range.

## Object literals

### `Const` Point

### ▪ **Point**: *object*

###  compare

▸ **compare**(`point`: [Point](../interfaces/_interfaces_point_.point.md), `another`: [Point](../interfaces/_interfaces_point_.point.md)): *-1 | 0 | 1*

Compare a point to another, returning an integer indicating whether the
point was before, at, or after the other.

**Parameters:**

Name | Type |
------ | ------ |
`point` | [Point](../interfaces/_interfaces_point_.point.md) |
`another` | [Point](../interfaces/_interfaces_point_.point.md) |

**Returns:** *-1 | 0 | 1*

###  equals

▸ **equals**(`point`: [Point](../interfaces/_interfaces_point_.point.md), `another`: [Point](../interfaces/_interfaces_point_.point.md)): *boolean*

Check if a point is exactly equal to another.

**Parameters:**

Name | Type |
------ | ------ |
`point` | [Point](../interfaces/_interfaces_point_.point.md) |
`another` | [Point](../interfaces/_interfaces_point_.point.md) |

**Returns:** *boolean*

###  isAfter

▸ **isAfter**(`point`: [Point](../interfaces/_interfaces_point_.point.md), `another`: [Point](../interfaces/_interfaces_point_.point.md)): *boolean*

Check if a point is after another.

**Parameters:**

Name | Type |
------ | ------ |
`point` | [Point](../interfaces/_interfaces_point_.point.md) |
`another` | [Point](../interfaces/_interfaces_point_.point.md) |

**Returns:** *boolean*

###  isBefore

▸ **isBefore**(`point`: [Point](../interfaces/_interfaces_point_.point.md), `another`: [Point](../interfaces/_interfaces_point_.point.md)): *boolean*

Check if a point is before another.

**Parameters:**

Name | Type |
------ | ------ |
`point` | [Point](../interfaces/_interfaces_point_.point.md) |
`another` | [Point](../interfaces/_interfaces_point_.point.md) |

**Returns:** *boolean*

###  isPoint

▸ **isPoint**(`value`: any): *value is Point*

Check if a value implements the `Point` interface.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is Point*

###  transform

▸ **transform**(`point`: [Point](../interfaces/_interfaces_point_.point.md), `op`: [Operation](_interfaces_operation_.md#operation), `options`: object): *[Point](../interfaces/_interfaces_point_.point.md) | null*

Transform a point by an operation.

**Parameters:**

▪ **point**: *[Point](../interfaces/_interfaces_point_.point.md)*

▪ **op**: *[Operation](_interfaces_operation_.md#operation)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`affinity?` | "forward" &#124; "backward" &#124; null |

**Returns:** *[Point](../interfaces/_interfaces_point_.point.md) | null*
