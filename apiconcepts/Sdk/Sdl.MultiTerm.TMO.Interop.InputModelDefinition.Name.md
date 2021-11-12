#  Name property

## Name

Sdl.MultiTerm.TMO.Interop.InputModelDefinition.Name —          Returns the name of the input model definition.

## Type

String
(read)

## Index Parameters
*none*

## Description

Each input model definition has a unique descriptive name. For example, this is the name that is listed in the input model list of MultiTerm Workstation.

All input model definitions can be referenced via this unique name.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select input model
InputModelDefinitions oInputModels = oTb.InputModelDefinitions;
for(int i=0;i<oInputModels.Count;i++)
{
   	Debug.WriteLine(oInputModels[i].Name);
}
```
