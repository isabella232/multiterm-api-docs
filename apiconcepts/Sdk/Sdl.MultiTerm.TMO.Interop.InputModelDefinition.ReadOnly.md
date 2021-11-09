

# 
    ReadOnly property



## Name

Sdl.MultiTerm.TMO.Interop.InputModelDefinition.ReadOnly —          Returns whether a particular input model definition is read-only.



## Type

Boolean

(read)



## Index Parameters
*none*


## Description



Input model definitions may be read-only, e.g. when the termbase administrator provides a central input model, which is not supposed to be altered by the end users. Via this property you can ascertain whether a particular input model is read-only for the currently logged-in user.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select input model
InputModelDefinitions oInputModels = oTb.InputModelDefinitions;
InputModelDefinition oInputModel = oInputModels["Default input model"];
Debug.WriteLine("Is the input model read-only for me? " + oInputModel.ReadOnly);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.InputModelDefinition.ReadOnly)

