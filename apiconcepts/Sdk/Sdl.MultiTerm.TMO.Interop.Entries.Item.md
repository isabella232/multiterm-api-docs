

# 
    Item method




## Name

Sdl.MultiTerm.TMO.Interop.Entries.Item —          Refers to a particular entry.



## Returntype
.md
[Sdl.MultiTerm.TMO.Interop.Entry](Sdl.MultiTerm.TMO.Interop.Entry.md)



## Parameters

* EntryID (Long)




## Description



Via this property you can retrieve a particular entry, e.g. to output the entire entry content. As parameter you need to provide the entry id of the corresponding entry.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//retrieve a particular entry
Entry oEntry = oEntries.Item(1);
//return full entry content
Debug.Write(oEntry.Content.Content);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Entries.Item)

