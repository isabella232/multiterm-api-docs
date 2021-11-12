# Term property

## Name
Sdl.MultiTerm.TMO.Interop.EntryIndex.Term —          Returns the term for the currently selected index.

## Type
String
(read / write)

## Index Parameters
*none*

## Description

Note that if, for example, the first available index contains two terms, these would be output like this:
```cs
///first 
term Debug.WriteLine(oIndexes[0].Term); 

///second 
term Debug.WriteLine(oIndexes[1].Term);
```


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

//output first term
Debug.WriteLine(oIndex.Term);
```
