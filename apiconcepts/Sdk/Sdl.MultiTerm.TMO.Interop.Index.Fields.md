# Fields property

## Name

Sdl.MultiTerm.TMO.Interop.Index.Fields —          Provides programmatic access to the entry-level descriptive fields.

## Type

[Sdl.MultiTerm.TMO.Interop.DescriptiveFields](Sdl.MultiTerm.TMO.Interop.DescriptiveFields.md)
(read)



## Index Parameters
*none*


## Description

An index can have descriptive fields assigned to it, i.e. fields that refer to all terms belonging to a particular index, e.g. "Definition." Via this property you can, for example, ascertain the number of such fields.



## Sample

```cs
Termbase oTb = oTbs["Termbase name"];

TermbaseDefinition oDef = oTb.Definition;
Indexes oIndexes = oDef.Indexes;

//select first index
Index oIndex = oIndexes[0];
DescriptiveFields oFields = oIndex.Fields;
Debug.WriteLine("Number of index-level descriptive fields: " + oFields.Count.ToString());
```

