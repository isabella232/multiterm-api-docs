# StartWizard method

## Name

Sdl.MultiTerm.TMO.Interop.ExportDefinition.StartWizard —          Calls up the export wizard for editing a particular export definition.

## Returntype

void

## Parameters

* XMLFileName (String, *optional*)
* SourceIndex (String, *optional, default is ""*)
* TargetIndex (String, *optional, default is ""*)



## Description


Applying this method to an export definition, opens the export wizard, which allows for GUI-based editing of the export definition. This method takes the name and path of an external export definition (\*.xdx) file as parameter. This means that you can provide an external export definition file to 'pre-fill' the wizard with some information. In addition you can provide the source/target language string parameters, as export definitions may use the source/target index as logical fields, e.g. an export definition that only exports source and target terms.

Note that the currently-logged in user needs to have permissions to edit the export definition in question, otherwise an error will be thrown.


## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select an export definition
ExportDefinitions oExpDefs = oTb.ExportDefinitions;
ExportDefinition oExpDef = oExpDefs["Default export definition"];
oExpDef.StartWizard("c:\\temp\\export.xdx", "English", "German");
```
