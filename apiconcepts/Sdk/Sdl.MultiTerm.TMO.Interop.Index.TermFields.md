# TermFields property

## Name

Sdl.MultiTerm.TMO.Interop.Index.TermFields —          Provides programmatic access to the term-level descriptive fields.

## Type
[Sdl.MultiTerm.TMO.Interop.DescriptiveFields](Sdl.MultiTerm.TMO.Interop.DescriptiveFields.md)
(read)



## Index Parameters
*none*


## Description



The termbase definition can contain descriptive fields that refer to a particular term, e.g. "Grammar." You can use this property to retrieve information on such fields, e.g. the number of available term-level fields.



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

TermbaseDefinition oDef = oTb.Definition;
Indexes oIndexes = oDef.Indexes;

//select first index
Index oIndex = oIndexes[0];
DescriptiveFields oFields = oIndex.TermFields;
Debug.WriteLine("Number of term-level descriptive fields: " + oFields.Count.ToString());
```

