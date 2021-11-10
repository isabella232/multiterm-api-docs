

# 
    ProcessExport method




## Name

Sdl.MultiTerm.TMO.Interop.ExportDefinition.ProcessExport —          Carries out the actual export process.



## Returntype

void



## Parameters
.md)
* Value ([Sdl.MultiTerm.TMO.Interop.MtTaskType](Sdl.MultiTerm.TMO.Interop.MtTaskType.md))
* SourceIndex (String, *optional, default is ""*)
* TargetIndex (String, *optional, default is ""*)




## Description



Applying this method to an export definition runs the export. It requires the task type as parameter, i.e. whether the export should be run in script mode (i.e. without the wizard) or using the export wizard. In addition you can provide the optional source/target index parameters. Note that export definitions can use the source/target index as logical fields, e.g. an export definition that only exports source and target terms.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select an export definition
ExportDefinitions oExpDefs = oTb.ExportDefinitions;
ExportDefinition oExpDef = oExpDefs["Default export definition"];
oExpDef.ProcessExport(Sdl.MultiTerm.TMO.Interop.MtTaskType.mtScript, "English", "German");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.ExportDefinition.ProcessExport)

