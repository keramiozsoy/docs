[slopes - v1.4.3](../README.md) › [Globals](../globals.md) › ["apis/avm/api"](../modules/_apis_avm_api_.md) › [PersistanceOptions](_apis_avm_api_.persistanceoptions.md)

# Class: PersistanceOptions

A class for defining the persistance behavior of this an API call.

## Hierarchy

* **PersistanceOptions**

## Index

### Constructors

* [constructor](_apis_avm_api_.persistanceoptions.md#constructor)

### Properties

* [mergeRule](_apis_avm_api_.persistanceoptions.md#protected-mergerule)
* [name](_apis_avm_api_.persistanceoptions.md#protected-name)
* [overwrite](_apis_avm_api_.persistanceoptions.md#protected-overwrite)

### Methods

* [getMergeRule](_apis_avm_api_.persistanceoptions.md#getmergerule)
* [getName](_apis_avm_api_.persistanceoptions.md#getname)
* [getOverwrite](_apis_avm_api_.persistanceoptions.md#getoverwrite)

## Constructors

###  constructor

\+ **new PersistanceOptions**(`name`: string, `overwrite`: boolean, `mergeRule`: [MergeRule](../modules/_apis_avm_types_.md#mergerule)): *[PersistanceOptions](_apis_avm_api_.persistanceoptions.md)*

*Defined in [apis/avm/api.ts:47](https://github.com/ava-labs/slopes/blob/709e172/src/apis/avm/api.ts#L47)*

**`remarks`** 
The merge rules are as follows:
  * "intersection" - the intersection of the set
  * "differenceSelf" - the difference between the existing data and new set
  * "differenceNew" - the difference between the new data and the existing set
  * "symDifference" - the union of the differences between both sets of data
  * "union" - the unique set of all elements contained in both sets
  * "unionMinusNew" - the unique set of all elements contained in both sets, excluding values only found in the new set
  * "unionMinusSelf" - the unique set of all elements contained in both sets, excluding values only found in the existing set

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`name` | string | - | The namespace of the database the data |
`overwrite` | boolean | false | True if the data should be completey overwritten |
`mergeRule` | [MergeRule](../modules/_apis_avm_types_.md#mergerule) | - | - |

**Returns:** *[PersistanceOptions](_apis_avm_api_.persistanceoptions.md)*

## Properties

### `Protected` mergeRule

• **mergeRule**: *[MergeRule](../modules/_apis_avm_types_.md#mergerule)* = "union"

*Defined in [apis/avm/api.ts:26](https://github.com/ava-labs/slopes/blob/709e172/src/apis/avm/api.ts#L26)*

___

### `Protected` name

• **name**: *string* =  undefined

*Defined in [apis/avm/api.ts:24](https://github.com/ava-labs/slopes/blob/709e172/src/apis/avm/api.ts#L24)*

___

### `Protected` overwrite

• **overwrite**: *boolean* = false

*Defined in [apis/avm/api.ts:25](https://github.com/ava-labs/slopes/blob/709e172/src/apis/avm/api.ts#L25)*

## Methods

###  getMergeRule

▸ **getMergeRule**(): *[MergeRule](../modules/_apis_avm_types_.md#mergerule)*

*Defined in [apis/avm/api.ts:45](https://github.com/ava-labs/slopes/blob/709e172/src/apis/avm/api.ts#L45)*

Returns the [MergeRule](../modules/_apis_avm_types_.md#mergerule) of the instance

**Returns:** *[MergeRule](../modules/_apis_avm_types_.md#mergerule)*

___

###  getName

▸ **getName**(): *string*

*Defined in [apis/avm/api.ts:31](https://github.com/ava-labs/slopes/blob/709e172/src/apis/avm/api.ts#L31)*

Returns the namespace of the instance

**Returns:** *string*

___

###  getOverwrite

▸ **getOverwrite**(): *boolean*

*Defined in [apis/avm/api.ts:38](https://github.com/ava-labs/slopes/blob/709e172/src/apis/avm/api.ts#L38)*

Returns the overwrite rule of the instance

**Returns:** *boolean*
