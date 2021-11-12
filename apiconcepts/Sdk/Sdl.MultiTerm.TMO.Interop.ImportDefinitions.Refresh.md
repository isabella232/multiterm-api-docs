# Refresh method

## Name

Sdl.MultiTerm.TMO.Interop.ImportDefinitions.Refresh —          Updates the import definition collection.

## Returntype

void

## Parameters
*none*

## Description

By applying this method you can make sure that MultiTerm client users always have access to the up-to-date import definition collection, which includes all definitions that have been added while the users were online.

## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

ImportDefinitions oImpDefs = oTb.ImportDefinitions;
oImpDefs.Refresh();
```
