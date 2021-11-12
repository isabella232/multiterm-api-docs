# LayoutDefinitions property


## Name
Sdl.MultiTerm.TMO.Interop.Termbase.LayoutDefinitions —          Provides programmatic access to the layout definitions of a termbase.


## Type

[Sdl.MultiTerm.TMO.Interop.LayoutDefinitions](Sdl.MultiTerm.TMO.Interop.LayoutDefinitions.md)
(read)



## Index Parameters
*none*

## Description


Layout definitions specify the entry layout, i.e. which fields to display, the field order and field formatting. After creation, each termbase is automatically assigned 5 default layout definitions. Users can add further layout definitions to suit special requirement (e.g. adapt the layout to an organisation's corporate identity). The layout definitions are physically stored in in the termbase.

Via this  property you can, for example, return the number of available layout definitions, generate a list with the names of the available layout definitions, etc.


## Sample


```cs
Termbase oTb = oTbs["Termbase Name"];

LayoutDefinitions oLayouts = oTb.LayoutDefinitions;

Debug.Write("Total number of layout definitions in termbase: " + oLayouts.Count.ToString());
```

