

# 
    IndexName property



## Name

Sdl.MultiTerm.TMO.Interop.EntryIndex.IndexName —          Returns the name of the selected index.



## Type

String

(read)



## Index Parameters
*none*


## Description



This property is used to return the name of the currently selected index, e.g. "English", "German", etc.



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

//return index name
Debug.WriteLine("Index name: " + oIndex.IndexName);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.EntryIndex.IndexName)

