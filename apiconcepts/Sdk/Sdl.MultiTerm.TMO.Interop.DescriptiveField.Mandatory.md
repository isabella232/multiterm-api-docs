

# 
    Mandatory property



## Name

Sdl.MultiTerm.TMO.Interop.DescriptiveField.Mandatory —          Returns whether the specified field is mandatory.



## Type

Boolean

(read)



## Index Parameters
*none*


## Description



The termbase creator/administrator can define descriptive fields in a termbase definition as mandatory, i.e. the user later has to fill in these fields before an entry can be saved. This property returns true if the field is mandatory, false if not.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//access termbase definition
TermbaseDefinition oDef = oTb.Definition;
//select first descriptive field
DescriptiveField oField = oDef.Fields[0];
Debug.WriteLine("Is this field mandatory? " + oField.Mandatory);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.DescriptiveField.Mandatory)

