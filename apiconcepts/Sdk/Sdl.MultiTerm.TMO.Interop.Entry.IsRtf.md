# IsRtf property

## Name

Sdl.MultiTerm.TMO.Interop.Entry.IsRtf —          Returns whether an entry is RTF.



## Type
Long
(read)

## Index Parameters
*none*


## Description

This property returns 0 if the current entry is not RTF, which will usually be the case.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry with id #1 
Entry oEntry = oEntries.Item(1);
Debug.Write("Is entry RTF? " + oEntry.IsRtf);
```


