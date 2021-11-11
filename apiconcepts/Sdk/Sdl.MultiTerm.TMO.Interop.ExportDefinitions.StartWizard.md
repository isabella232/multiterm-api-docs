# StartWizard method




## Name

Sdl.MultiTerm.TMO.Interop.ExportDefinitions.StartWizard —          Starts the Export Definition wizard.



## Returntype
[Sdl.MultiTerm.TMO.Interop.ExportDefinition](Sdl.MultiTerm.TMO.Interop.ExportDefinition.md)



## Parameters
*none*


## Description



Applying this method opens the Export Definition wizard, which allows you to create a new export definition with the wizard GUI.



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

ExportDefinitions oExpDefs = oTb.ExportDefinitions;
oExpDefs.StartWizard();
```

