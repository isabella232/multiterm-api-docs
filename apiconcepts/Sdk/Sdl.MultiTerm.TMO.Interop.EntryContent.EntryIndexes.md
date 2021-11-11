# EntryIndexes property

## Name

Sdl.MultiTerm.TMO.Interop.EntryContent.EntryIndexes —          Provides programmatic access to the indexes contained in a particular entry.

## Type

[Sdl.MultiTerm.TMO.Interop.EntryIndexes](Sdl.MultiTerm.TMO.Interop.EntryIndexes.md)

(read)



## Index Parameters
*none*


## Description

Each entry contains at least one index (i.e. one language). You can use the EntryIndexes class to retrieve the indexes and the terms contained in a particular entry, e.g. to return the number of entry indexes, the index labels and locales, etc.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry
Entry oEntry = oEntries.Item(1);
EntryContent content = oEntry.Content;

//loop through all terms in the entry
EntryIndexes oIndexes = content.EntryIndexes;
for(int i=0;i<oIndexes.Count;i++)
{
   	Debug.WriteLine(oIndexes[i].IndexName + ": " + oIndexes[i].Term);
}
```


