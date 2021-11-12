# StartWizard method

## Name

Sdl.MultiTerm.TMO.Interop.ImportDefinitions.StartWizard —          Starts the Import Definition wizard.

## Returntype
[Sdl.MultiTerm.TMO.Interop.ImportDefinition](Sdl.MultiTerm.TMO.Interop.ImportDefinition.md)

## Parameters
*none*


## Description

Applying this method opens the Import Definition wizard, which allows you to create a new import definition with the wizard GUI.


## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

ImportDefinitions oExpDefs = oTb.ImportDefinitions;
oImpDefs.StartWizard();
```

