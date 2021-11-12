# Load method

## Name

Sdl.MultiTerm.TMO.Interop.ExportDefinition.Load —          Updates the selected export definition from an external export definition file.

## Returntype
void


## Parameters

* FileName (String)


## Description

By applying this method to an export definition you can update the export definition from the content of an export definition (\*.xdx) file.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select an export definition
ExportDefinitions oExpDefs = oTb.ExportDefinitions;
ExportDefinition oExpDef = oExpDefs["Default export definition"];
oExpDef.Load("c:\\temp\\exp_def.xdx");
```

