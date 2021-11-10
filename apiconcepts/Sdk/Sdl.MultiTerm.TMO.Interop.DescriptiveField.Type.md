# Type property

## Name

Sdl.MultiTerm.TMO.Interop.DescriptiveField.Type —          Returns the descriptive field type.

## Type

[Sdl.MultiTerm.TMO.Interop.MtFieldType](Sdl.MultiTerm.TMO.Interop.MtFieldType.md)
(read)


## Index Parameters
*none*


## Description



Descriptive fields may be defined by the termbase creator/administrator as being of any of the following 6 types:



* text
* number
* boolean
* date/time
* picklist
* multimedia file


This property can, for example, be used to determine whether a specified field has the type value 4, i.e. whether it is a picklist field. In this case you can program your application to retrieve the corresponding picklist values.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//access termbase definition
TermbaseDefinition oDef = oTb.Definition;
//select first descriptive field
DescriptiveField oField = oDef.Fields[0];
Debug.WriteLine("Is this field multipe? " + oField.Type);
```


