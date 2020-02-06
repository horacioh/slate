[slate](../README.md) › [Globals](../globals.md) › ["utils/string"](_utils_string_.md)

# External module: "utils/string"

## Index

### Variables

* [CHAMELEON](_utils_string_.md#const-chameleon)
* [PUNCTUATION](_utils_string_.md#const-punctuation)
* [SPACE](_utils_string_.md#const-space)
* [SURROGATE_END](_utils_string_.md#const-surrogate_end)
* [SURROGATE_START](_utils_string_.md#const-surrogate_start)
* [ZERO_WIDTH_JOINER](_utils_string_.md#const-zero_width_joiner)

### Functions

* [getCharacterDistance](_utils_string_.md#const-getcharacterdistance)
* [getWordDistance](_utils_string_.md#const-getworddistance)
* [isBMPEmoji](_utils_string_.md#const-isbmpemoji)
* [isModifier](_utils_string_.md#const-ismodifier)
* [isSurrogate](_utils_string_.md#const-issurrogate)
* [isVariationSelector](_utils_string_.md#const-isvariationselector)
* [isWordCharacter](_utils_string_.md#const-iswordcharacter)

## Variables

### `Const` CHAMELEON

• **CHAMELEON**: *RegExp‹›* = /['\u2018\u2019]/

*Defined in [utils/string.ts:7](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/utils/string.ts#L7)*

___

### `Const` PUNCTUATION

• **PUNCTUATION**: *RegExp‹›* = /[\u0021-\u0023\u0025-\u002A\u002C-\u002F\u003A\u003B\u003F\u0040\u005B-\u005D\u005F\u007B\u007D\u00A1\u00A7\u00AB\u00B6\u00B7\u00BB\u00BF\u037E\u0387\u055A-\u055F\u0589\u058A\u05BE\u05C0\u05C3\u05C6\u05F3\u05F4\u0609\u060A\u060C\u060D\u061B\u061E\u061F\u066A-\u066D\u06D4\u0700-\u070D\u07F7-\u07F9\u0830-\u083E\u085E\u0964\u0965\u0970\u0AF0\u0DF4\u0E4F\u0E5A\u0E5B\u0F04-\u0F12\u0F14\u0F3A-\u0F3D\u0F85\u0FD0-\u0FD4\u0FD9\u0FDA\u104A-\u104F\u10FB\u1360-\u1368\u1400\u166D\u166E\u169B\u169C\u16EB-\u16ED\u1735\u1736\u17D4-\u17D6\u17D8-\u17DA\u1800-\u180A\u1944\u1945\u1A1E\u1A1F\u1AA0-\u1AA6\u1AA8-\u1AAD\u1B5A-\u1B60\u1BFC-\u1BFF\u1C3B-\u1C3F\u1C7E\u1C7F\u1CC0-\u1CC7\u1CD3\u2010-\u2027\u2030-\u2043\u2045-\u2051\u2053-\u205E\u207D\u207E\u208D\u208E\u2329\u232A\u2768-\u2775\u27C5\u27C6\u27E6-\u27EF\u2983-\u2998\u29D8-\u29DB\u29FC\u29FD\u2CF9-\u2CFC\u2CFE\u2CFF\u2D70\u2E00-\u2E2E\u2E30-\u2E3B\u3001-\u3003\u3008-\u3011\u3014-\u301F\u3030\u303D\u30A0\u30FB\uA4FE\uA4FF\uA60D-\uA60F\uA673\uA67E\uA6F2-\uA6F7\uA874-\uA877\uA8CE\uA8CF\uA8F8-\uA8FA\uA92E\uA92F\uA95F\uA9C1-\uA9CD\uA9DE\uA9DF\uAA5C-\uAA5F\uAADE\uAADF\uAAF0\uAAF1\uABEB\uFD3E\uFD3F\uFE10-\uFE19\uFE30-\uFE52\uFE54-\uFE61\uFE63\uFE68\uFE6A\uFE6B\uFF01-\uFF03\uFF05-\uFF0A\uFF0C-\uFF0F\uFF1A\uFF1B\uFF1F\uFF20\uFF3B-\uFF3D\uFF3F\uFF5B\uFF5D\uFF5F-\uFF65]/

*Defined in [utils/string.ts:6](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/utils/string.ts#L6)*

___

### `Const` SPACE

• **SPACE**: *RegExp‹›* = /\s/

*Defined in [utils/string.ts:5](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/utils/string.ts#L5)*

Constants for string distance checking.

___

### `Const` SURROGATE_END

• **SURROGATE_END**: *57343* = 57343

*Defined in [utils/string.ts:9](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/utils/string.ts#L9)*

___

### `Const` SURROGATE_START

• **SURROGATE_START**: *55296* = 55296

*Defined in [utils/string.ts:8](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/utils/string.ts#L8)*

___

### `Const` ZERO_WIDTH_JOINER

• **ZERO_WIDTH_JOINER**: *8205* = 8205

*Defined in [utils/string.ts:10](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/utils/string.ts#L10)*

## Functions

### `Const` getCharacterDistance

▸ **getCharacterDistance**(`text`: string): *number*

*Defined in [utils/string.ts:16](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/utils/string.ts#L16)*

Get the distance to the end of the first character in a string of text.

**Parameters:**

Name | Type |
------ | ------ |
`text` | string |

**Returns:** *number*

___

### `Const` getWordDistance

▸ **getWordDistance**(`text`: string): *number*

*Defined in [utils/string.ts:93](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/utils/string.ts#L93)*

Get the distance to the end of the first word in a string of text.

**Parameters:**

Name | Type |
------ | ------ |
`text` | string |

**Returns:** *number*

___

### `Const` isBMPEmoji

▸ **isBMPEmoji**(`code`: number): *boolean*

*Defined in [utils/string.ts:186](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/utils/string.ts#L186)*

Is `code` one of the BMP codes used in emoji sequences.

https://emojipedia.org/emoji-zwj-sequences/

**Parameters:**

Name | Type |
------ | ------ |
`code` | number |

**Returns:** *boolean*

___

### `Const` isModifier

▸ **isModifier**(`code`: number, `text`: string, `offset`: number): *boolean*

*Defined in [utils/string.ts:162](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/utils/string.ts#L162)*

Does `code` form Modifier with next one.

https://emojipedia.org/modifiers/

**Parameters:**

Name | Type |
------ | ------ |
`code` | number |
`text` | string |
`offset` | number |

**Returns:** *boolean*

___

### `Const` isSurrogate

▸ **isSurrogate**(`code`: number): *boolean*

*Defined in [utils/string.ts:153](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/utils/string.ts#L153)*

Determines if `code` is a surrogate

**Parameters:**

Name | Type |
------ | ------ |
`code` | number |

**Returns:** *boolean*

___

### `Const` isVariationSelector

▸ **isVariationSelector**(`code`: number): *boolean*

*Defined in [utils/string.ts:176](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/utils/string.ts#L176)*

Is `code` a Variation Selector.

https://codepoints.net/variation_selectors

**Parameters:**

Name | Type |
------ | ------ |
`code` | number |

**Returns:** *boolean*

___

### `Const` isWordCharacter

▸ **isWordCharacter**(`char`: string, `remaining`: string): *boolean*

*Defined in [utils/string.ts:124](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/utils/string.ts#L124)*

Check if a character is a word character. The `remaining` argument is used
because sometimes you must read subsequent characters to truly determine it.

**Parameters:**

Name | Type |
------ | ------ |
`char` | string |
`remaining` | string |

**Returns:** *boolean*
