

# 
    Item property




## Name

Sdl.MultiTerm.TMO.Interop.ExportDefinitions.Item —          Provides access to a particular export definition.



## Type
.md)
[Sdl.MultiTerm.TMO.Interop.ExportDefinition](Sdl.MultiTerm.TMO.Interop.ExportDefinition.md)

(read)



## Index Parameters

* Index (Variant)




## Description



To select a specific export definition you can either use the corresponding index number, e.g. Item(0), or the definition name, e.g. Item("Default export definition").



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

ExportDefinitions oExpDefs = oTb.ExportDefinitions;
ExportDefinition oExpDef = oExpDefs[0];
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.ExportDefinitions.Item)

