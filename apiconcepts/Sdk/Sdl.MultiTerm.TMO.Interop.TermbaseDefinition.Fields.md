

# 
    Fields property



## Name

Sdl.MultiTerm.TMO.Interop.TermbaseDefinition.Fields —          Provides access to entry-level fields.



## Type

[Sdl.MultiTerm.TMO.Interop.DescriptiveFields](Sdl.MultiTerm.TMO.Interop.DescriptiveFields.html)

(read)



## Index Parameters
*none*


## Description



Entry-level fields refer to the whole entry as such. Typically those are fields like "Subject", "Project", "Department", etc.

Via this class you can programmatically access entry-level fields defined in the termbase definition.



## Sample


```cs
Termbases oTbs = oLocalRep.Termbases;
Termbase oTb = oTbs["Termbase name"];

TermbaseDefinition tbDef = oTb.Definition;
Debug.Write("Number of entry-level fields in definition: " + tbDef.Fields.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseDefinition.Fields)

