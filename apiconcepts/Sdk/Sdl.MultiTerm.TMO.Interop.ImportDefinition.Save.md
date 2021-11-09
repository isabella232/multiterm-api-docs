

# 
    Save method



## Name

Sdl.MultiTerm.TMO.Interop.ImportDefinition.Save —          Saves the import definition to an external file.



## Returntype

void



## Parameters

* FileName (String)




## Description



Applying this method to a particular import definition saves the content of the import definition to an external file. Note that you need to provide the file path and name as well as the extension (\*.xdi) as parameter.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select an import definition
ImportDefinitions oImpDefs = oTb.ImportDefinitions;
ImportDefinition oImpDef = oImpDefs["Default import definition"];
oImpDef.Save("c:\\temp\\import.xdi");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.ImportDefinition.Save)

