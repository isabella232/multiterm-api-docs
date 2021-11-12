# Count property

## Name

Sdl.MultiTerm.TMO.Interop.LayoutDefinitions.Count —          Returns the number of available layout definitions.

## Type

Long
(read)

## Index Parameters
*none*
## Description

Via this property you can ascertain how many layout definitions are associated with a particular termbase.

## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

LayoutDefinitions oLayouts = oTb.LayoutDefinitions;
Debug.Write("Number of layout definitions: +" + oLayouts.Count);
```
