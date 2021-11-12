#  Name property

## Name

Sdl.MultiTerm.TMO.Interop.ExportDefinition.Name —          Returns the name of the export definition.

## Type
String
(read)


## Index Parameters
*none*


## Description

Each export definition has a unique descriptive name. For example, this is the name that is listed in the export definition list of the Termbase Catalogue in MultiTerm Workstation.

All export definitions can be referenced via this unique name.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select export definition
ExportDefinitions oExpDefs = oTb.ExportDefinitions;
ExportDefinition oExpDef;

//return list of export definition names
for(int i=0;i<oExpDefs.Count;i++)
{
   oExpDef = oExpDefs[i];
   Debug.WriteLine(oExpDef.Name);
}
```
