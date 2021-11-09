

# 
    ReadOnly property



## Name

Sdl.MultiTerm.TMO.Interop.EntryIndex.ReadOnly —          Indicates whether an index is read-only.



## Type

Boolean

(read)



## Index Parameters
*none*


## Description



Via this property you can ascertain whether a particular index is read-only for the currently logged-in user.



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

//see whether this index is read-only for currently logged-in user
Debug.WriteLine("Is index read-only: " + oIndex.ReadOnly);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.EntryIndex.ReadOnly)

