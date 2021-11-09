

# 
    Item property



## Name

Sdl.MultiTerm.TMO.Interop.LayoutDefinitions.Item —          Provides access to a particular layout definition.



## Type

[Sdl.MultiTerm.TMO.Interop.LayoutDefinition](Sdl.MultiTerm.TMO.Interop.LayoutDefinition.html)

(read)



## Index Parameters

* Index (Variant)




## Description



To select a specific layout definition you can either use the corresponding index number, e.g. Item(0), or the definition name, e.g. Item("Flags Layout").



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

LayoutDefinitions oLayouts = oTb.LayoutDefinitions;
LayoutDefinition oLayouts = oLayouts[0];
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.LayoutDefinitions.Item)
