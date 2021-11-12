# StartWizard method

## Name

Sdl.MultiTerm.TMO.Interop.ImportDefinition.StartWizard —          Calls up the import wizard for editing a particular import definition.


## Returntype

void

## Parameters

* XMLFileName (String, *optional*)
* SourceIndex (String, *optional, default is ""*)
* TargetIndex (String, *optional, default is ""*)

## Description

Applying this method to an import definition, opens the import wizard, which allows for GUI-based editing of the import definition. This method takes the name and path of an external import definition (\*.xdf) file as parameter. This means that you can provide an external import definition file to 'pre-fill' the wizard with information. In addition you can provide the source/target language string parameters, as import definitions may use the source/target index as logical fields.

Note that the currently-logged in user needs to have permissions to edit the import definition in question, otherwise an error will be thrown.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select an import definition
ImportDefinitions oImpDefs = oTb.ImportDefinitions;
ImportDefinition oImpDef = oImpDefs["Default import definition"];
oImpDef.StartWizard("c:\\temp\\import.xdi", "English", "German");
```


