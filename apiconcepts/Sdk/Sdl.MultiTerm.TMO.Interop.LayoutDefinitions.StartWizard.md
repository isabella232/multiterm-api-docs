# StartWizard method

## Name

Sdl.MultiTerm.TMO.Interop.LayoutDefinitions.StartWizard —          Starts the Layout Definition wizard.

## Returntype
[Sdl.MultiTerm.TMO.Interop.LayoutDefinition](Sdl.MultiTerm.TMO.Interop.LayoutDefinition.md)

## Parameters
*none*

## Description

Applying this method opens the Layout Definition, which allows you to create a new layout definition with the wizard GUI.

## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

LayoutDefinitions oLayouts = oTb.LayoutDefinitions;
oLayouts.StartWizard();
```

