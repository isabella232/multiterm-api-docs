

# 
    ImportDefinitions property



## Name

Sdl.MultiTerm.TMO.Interop.Termbase.ImportDefinitions —          Provides programmatic access to the filter definitions of a termbase.



## Type

[Sdl.MultiTerm.TMO.Interop.ImportDefinitions](Sdl.MultiTerm.TMO.Interop.ImportDefinitions.html)

(read)



## Index Parameters
*none*


## Description



Import definitions are used to import the content of external files (which are in MultiTerm XML format) into a selected termbase. Import definitions specify a number of import parameters, e.g. whether existing entries should be overwritten, merged, etc. After creation, each termbase is automatically assigned one default import definition. Administrative users (in the case of server-based termbases) can add further import definitions to suit special requirement. The import definitions are physically stored in in the termbase.

Via this property you can, for example, return the number of available import definitions, generate a list containing the names of the available import definitions, etc.



## Sample


```cs
Termbase oTb = oTbs["Termbase Name"];

ImportDefinitions oImpDefs = oTb.ImportDefinitions;

Debug.Write("Total number of import definitions in termbase: " + oImpDefs.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Termbase.ImportDefinitions)

