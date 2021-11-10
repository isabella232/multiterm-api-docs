

# 
    Item property




## Name

Sdl.MultiTerm.TMO.Interop.ImportDefinitions.Item —          Provides access to a particular import definition.



## Type
.md)
[Sdl.MultiTerm.TMO.Interop.ImportDefinition](Sdl.MultiTerm.TMO.Interop.ImportDefinition.md)

(read)



## Index Parameters

* Index (Variant)




## Description



To select a specific import definition you can either use the corresponding index number, e.g. Item(0), or the definition name, e.g. Item("Default import definition").



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

ImportDefinitions oImpDefs = oTb.ImportDefinitions;
ImportDefinition oImpDef = oImpDefs[0];
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.ImportDefinitions.Item)

