[slate](../README.md) › [Globals](../globals.md) › ["create-editor"](_create_editor_.md)

# External module: "create-editor"

## Index

### Functions

* [createEditor](_create_editor_.md#const-createeditor)
* [getDirtyPaths](_create_editor_.md#const-getdirtypaths)

## Functions

### `Const` createEditor

▸ **createEditor**(): *[Editor](../interfaces/_interfaces_editor_.editor.md)*

*Defined in [create-editor.ts:22](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/create-editor.ts#L22)*

Create a new Slate `Editor` object.

**Returns:** *[Editor](../interfaces/_interfaces_editor_.editor.md)*

___

### `Const` getDirtyPaths

▸ **getDirtyPaths**(`op`: [Operation](_interfaces_operation_.md#operation)): *number[][]*

*Defined in [create-editor.ts:301](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/create-editor.ts#L301)*

Get the "dirty" paths generated from an operation.

**Parameters:**

Name | Type |
------ | ------ |
`op` | [Operation](_interfaces_operation_.md#operation) |

**Returns:** *number[][]*
