# StartWizard method
## Name

Sdl.MultiTerm.TMO.Interop.InputModelDefinitions.StartWizard —          Starts the Input Model Definition wizard.

## Returntype
[Sdl.MultiTerm.TMO.Interop.InputModelDefinition](Sdl.MultiTerm.TMO.Interop.InputModelDefinition.md)

## Parameters
*none*

## Description

Applying this method opens the Input Model Definition wizard, which allows you to create a new input model definition with the wizard GUI.

## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

InputModelDefinitions oModels = oTb.InputModelDefinitions;
oModels.StartWizard();
```

