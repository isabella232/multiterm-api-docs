

# 
    Level property



## Name

Sdl.MultiTerm.TMO.Interop.DescriptiveField.Level —          Returns the descriptive field level value.



## Type

[Sdl.MultiTerm.TMO.Interop.MtFieldLevel](Sdl.MultiTerm.TMO.Interop.MtFieldLevel.html)

(read)



## Index Parameters
*none*


## Description



A descriptive field may apply on entry-level (i.e. it describes or categorises the entire entry), on index-level (i.e. it applies to all terms of a particular index), or it may be on term-level (i.e. it describes or categorises a specific term).

This property returns the field level value of a term in the termbase definition.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//access termbase definition
TermbaseDefinition oDef = oTb.Definition;
//select first descriptive field
DescriptiveField oField = oDef.Fields[0];
Debug.WriteLine(oField.Level);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.DescriptiveField.Level)

