# InputModelDefinitions property

## Name

Sdl.MultiTerm.TMO.Interop.Termbase.InputModelDefinitions —          Provides programmatic access to the input model definitions of a termbase.

## Type
[Sdl.MultiTerm.TMO.Interop.InputModelDefinitions](Sdl.MultiTerm.TMO.Interop.InputModelDefinitions.md)
(read)

## Index Parameters
*none*

## Description

Input models are a kind of template for creating new entries. Input models offer a way of structuring the input of data into a termbase to facilitate editing and to ensure a consistent entry structure throughout the termbase.

After creation, each termbase is automatically assigned one default input model definition. Users can add further input models as required. The input model definitions are physically stored in in the termbase.

Via the InputModelDefinitions property you can, for example, return the number of available input model definitions, generate a list that contains the names of the available input model definitions, etc.

## Sample


```cs
Termbase oTb = oTbs["Termbase Name"];

InputModelDefinitions  oModels = oTb.InputModelDefinitions;

Debug.Write("Total number of input models in termbase: " + oModels.Count.ToString());
```

