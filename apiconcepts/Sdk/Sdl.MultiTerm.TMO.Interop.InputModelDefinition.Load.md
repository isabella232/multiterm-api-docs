#  Load method
## Name

Sdl.MultiTerm.TMO.Interop.InputModelDefinition.Load —          Updates the selected input model from an external input model definition file.

## Returntype

void

## Parameters

* FileName (String)


## Description


By applying this method to an input model you can update the input model definition from the content of an input model definition (\*.xdm) file.


## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select input model
InputModelDefinitions oInputModels = oTb.InputModelDefinitions;
InputModelDefinition oInputModel = oInputModels["My own input model"];
oInputModel.Load("c:\\temp\\input_model.xdm");
```