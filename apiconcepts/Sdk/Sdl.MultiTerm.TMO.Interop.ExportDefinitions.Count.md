# Count property

## Name

Sdl.MultiTerm.TMO.Interop.ExportDefinitions.Count —          Returns the number of available export definitions.

## Type

Long
(read)

## Index Parameters
*none*


## Description

Via this property you can ascertain how many export definitions are associated with a particular termbase.

## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

ExportDefinitions oExpDefs = oTb.ExportDefinitions;
Debug.Write("Number of export definitions: +" + oExpDefs.Count);
```
