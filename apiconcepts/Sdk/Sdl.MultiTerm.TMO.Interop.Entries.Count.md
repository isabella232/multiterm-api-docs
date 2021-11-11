
# Count property

## Name

Sdl.MultiTerm.TMO.Interop.Entries.Count —          Returns the total number of termbase entries.

## Type

Long
(read)


## Index Parameters
*none*


## Description

You can use this property to ascertain the total number of entries contained in a particular termbase.


## Sample

```cs
Termbase oTb = oTbs["01test"];

Entries oEntries = oTb.Entries;
Debug.Write("Total entry count: " + oEntries.Count.ToString());
```


