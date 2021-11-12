#  Delete method

## Name

Sdl.MultiTerm.TMO.Interop.ExportDefinition.Delete —          Removes the export definition from the collection.

## Returntype
void

## Parameters
*none*


## Description

Applying this method removes the export definition  physically from the collection of export definitions. This can only be done, if the currently logged-in user is allowed to delete the export definition in question. If the user does not have the right to delete the export definition, a corresponding error message will be thrown. Users usually can only delete export definitions created by themselves.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select an export definition
ExportDefinitions oExpDefs = oTb.ExportDefinitions;
ExportDefinition oExpDef = oExpDefs["Default export definition"];
oExpDef.Delete();
```

