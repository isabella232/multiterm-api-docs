#  Multiple property

## Name

Sdl.MultiTerm.TMO.Interop.DescriptiveField.Multiple —          Returns whether a field can be multiple.

## Type

Boolean
(read)


## Index Parameters
*none*


## Description

A termbase creator/administrator can define descriptive fields in a termbase definition as multiple, i.e. the field may occur several times in an entry. If the field is not multiple, then only one occurrence of the field per entry is allowed.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//access termbase definition
TermbaseDefinition oDef = oTb.Definition;
//select first descriptive field
DescriptiveField oField = oDef.Fields[0];
Debug.WriteLine("Is this field multipe? " + oField.Multiple);
```
