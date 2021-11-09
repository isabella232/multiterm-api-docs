

# 
    Save method



## Name

Sdl.MultiTerm.TMO.Interop.InputModelDefinition.Save —          Saves the input model definition to an external file.



## Returntype

void



## Parameters

* FileName (String)




## Description



Applying this method to a particular input model saves the content of the input model definition to an external file. Note that you need to provide the file path and name as well as the extension (\*.xdm) as parameter.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select input model
InputModelDefinitions oInputModels = oTb.InputModelDefinitions;
InputModelDefinition oInputModel = oInputModels["My own input model"];
oInputModel.Save("c:\\temp\\input_model.xdm");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.InputModelDefinition.Save)

