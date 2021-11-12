# Description property

## Name

Sdl.MultiTerm.TMO.Interop.InputModelDefinition.Description —          Returns the input model definition description.

## Type

String
(read)

## Index Parameters
*none*

## Description

Each input model definition can have an optional description to provide further information on it. Via this property you can output the input model definition description string.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select input model
InputModelDefinitions oInputModels = oTb.InputModelDefinitions;
InputModelDefinition oInputModel = oInputModels["Default input model"];
Debug.WriteLine(oInputModel.Description);
```
