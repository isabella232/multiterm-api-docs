#  Count property

## Name

Sdl.MultiTerm.TMO.Interop.EntryIDs.Count —          Returns the number of entry ids contained in a termbase.

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

//get entry ids
EntryIDs oIds = oTb.Entries.GetEntryIDs();
Debug.WriteLine(oIds.Count.ToString());
```

