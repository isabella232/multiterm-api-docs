

# 
    Load method



## Name

Sdl.MultiTerm.TMO.Interop.ImportDefinition.Load —          Updates the selected import definition from an external import definition file.



## Returntype

void



## Parameters

* FileName (String)




## Description



By applying this method to an import definition you can update the import definition from the content of an import definition (\*.xdi) file.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select an import definition
ImportDefinitions oImpDefs = oTb.ImportDefinitions;
ImportDefinition oExpDef = oImpDefs["Default import definition"];
oImpDef.Load("c:\\temp\\imp_def.xdi");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.ImportDefinition.Load)

