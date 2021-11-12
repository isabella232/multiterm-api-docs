# ReadOnly property

## Name

Sdl.MultiTerm.TMO.Interop.ExportDefinition.ReadOnly —          Returns whether a particular export definition is read-only.

## Type

Boolean
(read)

## Index Parameters
*none*

## Description

Export definitions may be read-only, e.g. when the termbase administrator provides a central export definition, which is not supposed to be altered by the end users. Via this property you can ascertain whether a particular export definition is read-only for the currently logged-in user.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select an export definition
ExportDefinitions oExpDefs = oTb.ExportDefinitions;
ExportDefinition oExpDef = oExpDefs["Default export definition"];
Debug.WriteLine("Is this export definition read-only for me? " + oExpDef.ReadOnly);
```
