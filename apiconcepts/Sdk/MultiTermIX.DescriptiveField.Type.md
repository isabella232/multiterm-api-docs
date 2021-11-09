

# 
    Type property



## Name

MultiTermIX.DescriptiveField.Type —          Returns the descriptive field type.



## Type

[MultiTermIX.MtFieldType](MultiTermIX.MtFieldType.html)

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



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20MultiTermIX.DescriptiveField.Type)

