

# 
    ProcessImport method




## Name

Sdl.MultiTerm.TMO.Interop.ImportDefinition.ProcessImport —          Carries out the actual import process.



## Returntype

void



## Parameters
.md)
* Value ([Sdl.MultiTerm.TMO.Interop.MtTaskType](Sdl.MultiTerm.TMO.Interop.MtTaskType.md))
* SourceIndex (String, *optional, default is ""*)
* TargetIndex (String, *optional, default is ""*)




## Description



Applying this method to an import definition runs the import. It requires the task type as parameter, i.e. whether the import should be run in script mode (i.e. without the wizard) or using the import wizard. In addition you can provide the optional source/target index parameters. Note that import definitions can use the source/target index as logical fields.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select an import definition
ImportDefinitions oImpDefs = oTb.ImportDefinitions;
ImportDefinition oExpDef = oImpDefs["Default import definition"];
oImpDef.ProcessImport(Sdl.MultiTerm.TMO.Interop.MtTaskType.mtScript, "English", "German");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.ImportDefinition.ProcessImport)

