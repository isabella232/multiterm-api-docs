# StartWizard method

## Name

Sdl.MultiTerm.TMO.Interop.InputModelDefinition.StartWizard —          Calls up the input model wizard for editing a particular input model.

## Returntype

void

## Parameters

* XMLFileName (String, *optional*)


## Description

Applying this method to an input model, opens the input model wizard, which allows for GUI-based editing of the input model. This method takes the name and path of an external input model definition (\*.xdm) file as parameter. This means that you can provide an external input model definition file to 'pre-fill' the wizard with some information.

Note that the currently-logged in user needs to have permissions to edit the input model definition in question, otherwise an error will be thrown.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select input model
InputModelDefinitions oInputModels = oTb.InputModelDefinitions;
InputModelDefinition oInputModel = oInputModels["My own input model"];
oInputModel.StartWizard("c:\\temp\\input_model.xdm");
```
