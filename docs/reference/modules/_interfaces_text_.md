
# External module: "interfaces/text"

## Index

### Interfaces

* [Text](../interfaces/_interfaces_text_.text.md)

### Object literals

* [Text](_interfaces_text_.md#const-text)

## Object literals

### `Const` Text

### ▪ **Text**: *object*

###  decorations

▸ **decorations**(`node`: [Text](../interfaces/_interfaces_text_.text.md), `decorations`: [Range](../interfaces/_interfaces_range_.range.md)[]): *[Text](../interfaces/_interfaces_text_.text.md)[]*

Get the leaves for a text node given decorations.

**Parameters:**

Name | Type |
------ | ------ |
`node` | [Text](../interfaces/_interfaces_text_.text.md) |
`decorations` | [Range](../interfaces/_interfaces_range_.range.md)[] |

**Returns:** *[Text](../interfaces/_interfaces_text_.text.md)[]*

###  equals

▸ **equals**(`text`: [Text](../interfaces/_interfaces_text_.text.md), `another`: [Text](../interfaces/_interfaces_text_.text.md), `options`: object): *boolean*

Check if two text nodes are equal.

**Parameters:**

▪ **text**: *[Text](../interfaces/_interfaces_text_.text.md)*

▪ **another**: *[Text](../interfaces/_interfaces_text_.text.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`loose?` | boolean |

**Returns:** *boolean*

###  isText

▸ **isText**(`value`: any): *value is Text*

Check if a value implements the `Text` interface.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is Text*

###  isTextList

▸ **isTextList**(`value`: any): *value is Text[]*

Check if a value is a list of `Text` objects.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is Text[]*

###  matches

▸ **matches**(`text`: [Text](../interfaces/_interfaces_text_.text.md), `props`: Partial‹[Text](../interfaces/_interfaces_text_.text.md)›): *boolean*

Check if an text matches set of properties.

Note: this is for matching custom properties, and it does not ensure that
the `text` property are two nodes equal.

**Parameters:**

Name | Type |
------ | ------ |
`text` | [Text](../interfaces/_interfaces_text_.text.md) |
`props` | Partial‹[Text](../interfaces/_interfaces_text_.text.md)› |

**Returns:** *boolean*
