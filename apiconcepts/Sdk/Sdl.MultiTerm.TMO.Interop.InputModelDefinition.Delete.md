

# 
    Delete method



## Name

Sdl.MultiTerm.TMO.Interop.InputModelDefinition.Delete —          Removes the input model definition from the collection.



## Returntype

void



## Parameters
*none*


## Description



Applying this method removes the input model physically from the collection of input model definitions. This can only be done, if the currently logged-in user is allowed to delete the input model in question. If the user does not have the right to delete the input model, a corresponding error message will be thrown. Users usually can only delete input models created by themselves.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select input model
InputModelDefinitions oInputModels = oTb.InputModelDefinitions;
InputModelDefinition oInputModel = oInputModels["My own input model"];
oInputModel.Delete();
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.InputModelDefinition.Delete)

