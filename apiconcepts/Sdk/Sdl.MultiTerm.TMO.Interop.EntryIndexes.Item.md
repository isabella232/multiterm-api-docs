

# 
    Item property




## Name

Sdl.MultiTerm.TMO.Interop.EntryIndexes.Item —          Refers to a particular entry index.



## Type
.md)
[Sdl.MultiTerm.TMO.Interop.EntryIndex](Sdl.MultiTerm.TMO.Interop.EntryIndex.md)

(read)



## Index Parameters

* Index (Variant)




## Description



This property is used to select a particular index from the entry index collection. You can either use the index number, e.g. oIndexes[0] or the actual index name as parameter, e.g. oIndexes["English"]. It is recommended to use the index number, as an index (language) can contain more than one term. For example, if an entry has two languages and if each language has two terms, the last term will be referred to as oIndexes[3].Term.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry #1
Entry oEntry = oEntries.Item(1);
EntryIndexes oIndexes = oEntry.Content.EntryIndexes;
Debug.WriteLine(oIndexes[0].Term);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.EntryIndexes.Item)

