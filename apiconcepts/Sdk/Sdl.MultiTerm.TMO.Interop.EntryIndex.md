

# 
    Sdl.MultiTerm.TMO.Interop.EntryIndex class




## Name

Sdl.MultiTerm.TMO.Interop.EntryIndex —          Provides programmatic access to a particular index.



## Description



Via this class you can access a particular index, e.g. in order to retrieve any descriptive fields associated with the index, term-level descriptive fields, etc.



## Properties
.md)
* [IndexFields](Sdl.MultiTerm.TMO.Interop.EntryIndex.IndexFields.md): Provides programmatic access to the descriptive fields of an index.
* [IndexName](Sdl.MultiTerm.TMO.Interop.EntryIndex.IndexName.md): Returns the name of the selected index.
* [ReadOnly](Sdl.MultiTerm.TMO.Interop.EntryIndex.ReadOnly.md): Indicates whether an index is read-only.
* [Term](Sdl.MultiTerm.TMO.Interop.EntryIndex.Term.md): Returns the term for the currently selected index.
* [TermFields](Sdl.MultiTerm.TMO.Interop.EntryIndex.TermFields.md): Provides programmatic access to the term-level descriptive fields.




## Methods
*None*


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

Debug.WriteLine(oIndex.Term);
Debug.WriteLine("Number of index-level descriptive fields: " + oIndex.IndexFields.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.EntryIndex)

