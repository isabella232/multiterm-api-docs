# Add method

## Name

Sdl.MultiTerm.TMO.Interop.InputModelDefinitions.Add —          Adds a new input model definition to the collection.

## Returntype
[Sdl.MultiTerm.TMO.Interop.InputModelDefinition](Sdl.MultiTerm.TMO.Interop.InputModelDefinition.md)

## Parameters

* Name (String)
* Description (String)
* FileName (String)

## Description

Applying this method to an input model definition collection adds a new input model definition from an input model definition that was saved as an external \*.xdm file. This method requires the name of the new input model definition, an optional description and the full path and name of the input model definition file.

## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

InputModelDefinitions oModels = oTb.InputModelDefinitions;
oModels.Add("Input model name", "Input model description", "c:\\temp\\def_model.xdm");
```
