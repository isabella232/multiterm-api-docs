

# 
    ApplyExport method



## Name

Sdl.MultiTerm.TMO.Interop.Entry.ApplyExport —          Exports a particular entry.



## Returntype

String



## Parameters

* ExportDefinition ([Sdl.MultiTerm.TMO.Interop.ExportDefinition](Sdl.MultiTerm.TMO.Interop.ExportDefinition.html))
* SourceIndex (String, *optional, default is ""*)
* TargetIndex (String, *optional, default is ""*)




## Description



Export definitions are used to export termbase entries to an external file according to the specifications of the corresponding export definition.

Applying a selected export definition to a particular entry programmatically does not actually export the selected entry to an external file. It rather generates a string output in the format specified by the selected export definition (e.g. XML, TXT, RTF), which can then, for example, be written into an external file.

Thos method requires an export definition object as parameter. Export definitions can be selected either via the corresponding index number or via the unique termbase object name, which is case-sensitive, e.g. ExportDefinitions["Default export definition"] or ExportDefinitions[0].

Additionally you also need to provide the source and target index, as some export definitions rely on that information, e.g. custom export definitions that specify that only the current source and target terms should be exported.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry with id #1 
Entry oEntry = oEntries.Item(1);

//select export definition
ExportDefinitions oExpDefs = oTb.ExportDefinitions;
ExportDefinition oExpDef = oExpDefs["Default export definition"];

//apply export definition
string result =oEntry.ApplyExport(oExpDef, "English", "German");
Debug.Write(result);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Entry.ApplyExport)

