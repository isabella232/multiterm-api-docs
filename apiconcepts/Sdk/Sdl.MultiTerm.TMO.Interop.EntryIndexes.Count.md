#  Count property

## Name

Sdl.MultiTerm.TMO.Interop.EntryIndexes.Count —          Returns the number of indexes contained in a particular entry.

## Type
Long
(read)

## Index Parameters
*none*

## Description


## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry #1
Entry oEntry = oEntries.Item(1);
EntryIndexes oIndexes = oEntry.Content.EntryIndexes;
Debug.WriteLine("Number of indexes/terms in the current entry:" + oIndexes.Count.ToString());
```
