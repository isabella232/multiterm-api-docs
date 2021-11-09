

# 
    Content property



## Name

Sdl.MultiTerm.TMO.Interop.Entry.Content —          Provides access to the content of an entry.



## Type

[Sdl.MultiTerm.TMO.Interop.EntryContent](Sdl.MultiTerm.TMO.Interop.EntryContent.html)

(read)



## Index Parameters
*none*


## Description



You can use this property to return the content of an entry fully or partially, e.g. only the content of a specific index.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry with id #1 and output entry content
Entry oEntry = oEntries.Item(1);
Debug.Write(oEntry.Content.Content);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Entry.Content)

