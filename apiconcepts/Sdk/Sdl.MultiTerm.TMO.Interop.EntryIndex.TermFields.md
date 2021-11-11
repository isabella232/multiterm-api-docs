# TermFields property


## Name

Sdl.MultiTerm.TMO.Interop.EntryIndex.TermFields —          Provides programmatic access to the term-level descriptive fields.



## Type
[Sdl.MultiTerm.TMO.Interop.EntryFields](Sdl.MultiTerm.TMO.Interop.EntryFields.md)

(read)



## Index Parameters
*none*


## Description



By applying this property you can retrieve the descriptive fields associated with the term (if any). Descriptive fields are used to categorise and describe a specific term (e.g. "Grammar", "Definition", "Note", etc.)



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry #1
Entry oEntry = oEntries.Item(1);

EntryIndexes oIndexes = oEntry.Content.EntryIndexes;

//select first entry index
EntryIndex oIndex = oIndexes[0];

//return number of descriptive fields for the first term
Debug.WriteLine("Number of term-level descriptive fields: " + oIndex.TermFields.Count.ToString());
```
