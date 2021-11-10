

# 
    IndexFields property




## Name

Sdl.MultiTerm.TMO.Interop.EntryIndex.IndexFields —          Provides programmatic access to the descriptive fields of an index.



## Type
.md)
[Sdl.MultiTerm.TMO.Interop.EntryFields](Sdl.MultiTerm.TMO.Interop.EntryFields.md)

(read)



## Index Parameters
*none*


## Description



An index in an entry can have descriptive fields, which apply to all the terms contained in an index, e.g. a "Definition" field that provides information on the (synonymous) terms of an index.

By applying this  property to a specific index you can retrieve the descriptive fields associated with it (if any) with their respective labels, values, etc.



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

//access index-level descriptive fields
Debug.WriteLine("Number of index-level descriptive fields: " + oIndex.IndexFields.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.EntryIndex.IndexFields)

