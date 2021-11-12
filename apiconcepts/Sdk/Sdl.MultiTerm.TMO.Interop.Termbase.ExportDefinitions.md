# ExportDefinitions property


## Name

Sdl.MultiTerm.TMO.Interop.Termbase.ExportDefinitions —          Provides programmatic access to the export definitions of a termbase.


## Type

[Sdl.MultiTerm.TMO.Interop.ExportDefinitions](Sdl.MultiTerm.TMO.Interop.ExportDefinitions.md)
(read)


## Index Parameters
*none*

## Description

Export definitions are used to export termbase content to an external file. Depending on the export definition the output file may be in MultiTerm XML or in a different format (e.g. HTML). After creation, each termbase is automatically assigned 5 default export definitions. Administrative users (in the case of server-based termbases) can add further export definitions to suit special requirement. Export definitions are physically stored in in the termbase.

Via this property you can, for example, return the number of available export definitions, generate a list containing the names of available export definitions, etc.


## Sample


```cs
Termbase oTb = oTbs["Termbase Name"];

ExportDefinitions oExpDefs = oTb.ExportDefinitions;

Debug.Write("Total number of export definitions in termbase: " + oExpDefs.Count.ToString());
```


