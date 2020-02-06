
# External module: "interfaces/element"

## Index

### Interfaces

* [Element](../interfaces/_interfaces_element_.element.md)

### Type aliases

* [ElementEntry](_interfaces_element_.md#elemententry)

### Object literals

* [Element](_interfaces_element_.md#const-element)

## Type aliases

###  ElementEntry

Ƭ **ElementEntry**: *[[Element](../interfaces/_interfaces_element_.element.md), [Path](_interfaces_path_.md#path)]*

`ElementEntry` objects refer to an `Element` and the `Path` where it can be
found inside a root node.

## Object literals

### `Const` Element

### ▪ **Element**: *object*

###  isElement

▸ **isElement**(`value`: any): *value is Element*

Check if a value implements the `Element` interface.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is Element*

###  isElementList

▸ **isElementList**(`value`: any): *value is Element[]*

Check if a value is an array of `Element` objects.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is Element[]*

###  matches

▸ **matches**(`element`: [Element](../interfaces/_interfaces_element_.element.md), `props`: Partial‹[Element](../interfaces/_interfaces_element_.element.md)›): *boolean*

Check if an element matches set of properties.

Note: this checks custom properties, and it does not ensure that any
children are equivalent.

**Parameters:**

Name | Type |
------ | ------ |
`element` | [Element](../interfaces/_interfaces_element_.element.md) |
`props` | Partial‹[Element](../interfaces/_interfaces_element_.element.md)› |

**Returns:** *boolean*
