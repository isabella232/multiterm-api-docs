#  Item property

## Name

Sdl.MultiTerm.TMO.Interop.PicklistValues.Item —          Refers to a specific value from the picklist of a specified picklist field.

## Type

String
(read)

## Index Parameters

* Index (Long)

## Description

This property is used to retrieve a specific value from a picklist field. You may use it, for example, to loop through a picklist and return each picklist value from the termbase definition.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//access termbase definition
TermbaseDefinition oDef = oTb.Definition;
//select first descriptive field
DescriptiveField oField = oDef.Fields[0];
//generate list of picklist values
PicklistValues oValues = oField.PicklistValues;
Debug.WriteLine("First picklist value: " + oValues[0]);
```
