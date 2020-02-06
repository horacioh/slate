[slate](../README.md) › [Globals](../globals.md) › ["interfaces/text"](_interfaces_text_.md)

# External module: "interfaces/text"

## Index

### Interfaces

* [Text](../interfaces/_interfaces_text_.text.md)

### Object literals

* [Text](_interfaces_text_.md#const-text)

## Object literals

### `Const` Text

### ▪ **Text**: *object*

*Defined in [interfaces/text.ts:15](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/text.ts#L15)*

###  decorations

▸ **decorations**(`node`: [Text](../interfaces/_interfaces_text_.text.md), `decorations`: [Range](../interfaces/_interfaces_range_.range.md)[]): *[Text](../interfaces/_interfaces_text_.text.md)[]*

*Defined in [interfaces/text.ts:91](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/text.ts#L91)*

Get the leaves for a text node given decorations.

**Parameters:**

Name | Type |
------ | ------ |
`node` | [Text](../interfaces/_interfaces_text_.text.md) |
`decorations` | [Range](../interfaces/_interfaces_range_.range.md)[] |

**Returns:** *[Text](../interfaces/_interfaces_text_.text.md)[]*

###  equals

▸ **equals**(`text`: [Text](../interfaces/_interfaces_text_.text.md), `another`: [Text](../interfaces/_interfaces_text_.text.md), `options`: object): *boolean*

*Defined in [interfaces/text.ts:20](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/text.ts#L20)*

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

*Defined in [interfaces/text.ts:54](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/text.ts#L54)*

Check if a value implements the `Text` interface.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is Text*

###  isTextList

▸ **isTextList**(`value`: any): *value is Text[]*

*Defined in [interfaces/text.ts:62](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/text.ts#L62)*

Check if a value is a list of `Text` objects.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is Text[]*

###  matches

▸ **matches**(`text`: [Text](../interfaces/_interfaces_text_.text.md), `props`: Partial‹[Text](../interfaces/_interfaces_text_.text.md)›): *boolean*

*Defined in [interfaces/text.ts:73](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/text.ts#L73)*

Check if an text matches set of properties.

Note: this is for matching custom properties, and it does not ensure that
the `text` property are two nodes equal.

**Parameters:**

Name | Type |
------ | ------ |
`text` | [Text](../interfaces/_interfaces_text_.text.md) |
`props` | Partial‹[Text](../interfaces/_interfaces_text_.text.md)› |

**Returns:** *boolean*
