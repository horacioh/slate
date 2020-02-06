[slate](../README.md) › [Globals](../globals.md) › ["interfaces/point"](_interfaces_point_.md)

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

*Defined in [interfaces/point.ts:160](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/point.ts#L160)*

`PointEntry` objects are returned when iterating over `Point` objects that
belong to a range.

## Object literals

### `Const` Point

### ▪ **Point**: *object*

*Defined in [interfaces/point.ts:18](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/point.ts#L18)*

###  compare

▸ **compare**(`point`: [Point](../interfaces/_interfaces_point_.point.md), `another`: [Point](../interfaces/_interfaces_point_.point.md)): *-1 | 0 | 1*

*Defined in [interfaces/point.ts:24](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/point.ts#L24)*

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

*Defined in [interfaces/point.ts:56](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/point.ts#L56)*

Check if a point is exactly equal to another.

**Parameters:**

Name | Type |
------ | ------ |
`point` | [Point](../interfaces/_interfaces_point_.point.md) |
`another` | [Point](../interfaces/_interfaces_point_.point.md) |

**Returns:** *boolean*

###  isAfter

▸ **isAfter**(`point`: [Point](../interfaces/_interfaces_point_.point.md), `another`: [Point](../interfaces/_interfaces_point_.point.md)): *boolean*

*Defined in [interfaces/point.ts:40](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/point.ts#L40)*

Check if a point is after another.

**Parameters:**

Name | Type |
------ | ------ |
`point` | [Point](../interfaces/_interfaces_point_.point.md) |
`another` | [Point](../interfaces/_interfaces_point_.point.md) |

**Returns:** *boolean*

###  isBefore

▸ **isBefore**(`point`: [Point](../interfaces/_interfaces_point_.point.md), `another`: [Point](../interfaces/_interfaces_point_.point.md)): *boolean*

*Defined in [interfaces/point.ts:48](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/point.ts#L48)*

Check if a point is before another.

**Parameters:**

Name | Type |
------ | ------ |
`point` | [Point](../interfaces/_interfaces_point_.point.md) |
`another` | [Point](../interfaces/_interfaces_point_.point.md) |

**Returns:** *boolean*

###  isPoint

▸ **isPoint**(`value`: any): *value is Point*

*Defined in [interfaces/point.ts:67](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/point.ts#L67)*

Check if a value implements the `Point` interface.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is Point*

###  transform

▸ **transform**(`point`: [Point](../interfaces/_interfaces_point_.point.md), `op`: [Operation](_interfaces_operation_.md#operation), `options`: object): *[Point](../interfaces/_interfaces_point_.point.md) | null*

*Defined in [interfaces/point.ts:79](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/point.ts#L79)*

Transform a point by an operation.

**Parameters:**

▪ **point**: *[Point](../interfaces/_interfaces_point_.point.md)*

▪ **op**: *[Operation](_interfaces_operation_.md#operation)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`affinity?` | "forward" &#124; "backward" &#124; null |

**Returns:** *[Point](../interfaces/_interfaces_point_.point.md) | null*
