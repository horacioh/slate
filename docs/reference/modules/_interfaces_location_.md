
# External module: "interfaces/location"

## Index

### Type aliases

* [Location](_interfaces_location_.md#location)
* [Span](_interfaces_location_.md#span)

### Object literals

* [Location](_interfaces_location_.md#const-location)
* [Span](_interfaces_location_.md#const-span)

## Type aliases

###  Location

Ƭ **Location**: *[Path](_interfaces_path_.md#path) | [Point](../interfaces/_interfaces_point_.point.md) | [Range](../interfaces/_interfaces_range_.range.md)*

The `Location` interface is a union of the ways to refer to a specific
location in a Slate document: paths, points or ranges.

Methods will often accept a `Location` instead of requiring only a `Path`,
`Point` or `Range`. This eliminates the need for developers to manage
converting between the different interfaces in their own code base.

___

###  Span

Ƭ **Span**: *[[Path](_interfaces_path_.md#path), [Path](_interfaces_path_.md#path)]*

The `Span` interface is a low-level way to refer to locations in nodes
without using `Point` which requires leaf text nodes to be present.

## Object literals

### `Const` Location

### ▪ **Location**: *object*

###  isLocation

▸ **isLocation**(`value`: any): *value is Location*

Check if a value implements the `Location` interface.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is Location*

___

### `Const` Span

### ▪ **Span**: *object*

###  isSpan

▸ **isSpan**(`value`: any): *value is Span*

Check if a value implements the `Span` interface.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is Span*
